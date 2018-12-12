<template>
  <div class="child">
    <p>{{ testData }}</p>
    <button v-on:click='changeTestData'>change test</button>
  </div>
</template>

<script>
export default {
  name: 'Child',
  props: {
    testData: String,
    changeTestData: Function
  }
}
</script>
