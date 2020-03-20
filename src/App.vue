<template>
  <div id="app">

    <div class='checker'>
      <input type='checkbox' id='show-v-date-picker' v-model='showVDatePicker'/>
      <label for='show-v-date-picker'>Show v-date-picker test</label>
    </div>
    <v-cal-date-picker v-show='showVDatePicker'></v-cal-date-picker>

    <div class='checker'>
      <input type='checkbox' id='show-ctk-picker' v-model='showCtkPicker'/>
      <label for='show-ctk-picker'>Show vue-ctk-date-time-picker test</label>
    </div>
    <ctk-date-time-picker v-show='showCtkPicker'></ctk-date-time-picker>

    <div class='checker'>
      <input type='checkbox' id='show-functional-cal' v-model='showFunctionalCal'/>
      <label for='show-functional-cal'>Show vue-functional-calendar test</label>
    </div>
    <functional-cal v-show='showFunctionalCal'></functional-cal>

    <div class='checker'>
      <input type='checkbox' id='show-date-pick' v-model='showDatePick'/>
      <label for='show-date-pick'>Show vue-date-pick test</label>
    </div>
    <date-pick-test v-show='showDatePick'></date-pick-test>
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
  },
  data() {
    return {
      showVDatePicker: false,
      showCtkPicker: false,
      showFunctionalCal: false,
      showDatePick: false,
    };
  },
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
.checker {
  display: flex;
  margin: 20px;
}
</style>
