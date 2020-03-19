<template>
  <div id="app">
    <VCalDatePicker></VCalDatePicker>
    <CtkDateTimePicker></CtkDateTimePicker>
  </div>
</template>

<script>
import VCalDatePicker from './components/VCalDatePicker.vue';
import CtkDateTimePicker from './components/CtkDateTimePicker.vue';

export default {
  name: 'App',
  components: {
    VCalDatePicker,
    CtkDateTimePicker,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
