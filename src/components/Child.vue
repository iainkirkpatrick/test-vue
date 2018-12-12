<template>
  <div class="child">
    <p>msg is: {{ msg }}</p>
    <p>testData is: {{ testData }}</p>
    <button v-on:click='changeTestData'>change test data</button>
    <button v-on:click='changeMsg'>change msg</button>
  </div>
</template>

<script>
export default {
  name: 'Child',
  props: {
    msg: String,
    testData: String,
    changeMsg: Function,
    changeTestData: Function
  }
}
</script>
