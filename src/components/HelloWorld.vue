<template>
  <div class="hello">
    <Child :testData='testData' :changeTestData='changeTestData' />
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
      this.testData = 'another test'
    }
  }
}
</script>
