<template>
  <div class="hello">
    <Child
      :msg='msg'
      :testData='testData'
      :changeMsg='changeMsg'
      :changeTestData='changeTestData'
    />
  </div>
</template>

<script>
import Child from './Child.vue'

export default {
  name: 'HelloWorld',
  components: {
    Child
  },
  props: {
    msg: String
  },
  data: function () {
    return {
      testData: 'a test'
    }
  },
  methods: {
    changeTestData: function () {
      this.testData = 'new testData'
    },
    changeMsg: function () {
      this.msg = 'a new message'
    }
  }
}
</script>
