<template>
  <div id="app">
    <VCalDatePicker></VCalDatePicker>
    <CtkDateTimePicker></CtkDateTimePicker>
    <FunctionalCal></FunctionalCal>
    <date-pick-test/>
  </div>
</template>

<script>
import VCalDatePicker from './components/VCalDatePicker.vue';
import CtkDateTimePicker from './components/CtkDateTimePicker.vue';
import FunctionalCal from './components/FunctionalCal.vue';
import DatePickTest from './components/DatePickTest.vue';

export default {
  name: 'App',
  components: {
    VCalDatePicker,
    CtkDateTimePicker,
    FunctionalCal,
    DatePickTest,
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
