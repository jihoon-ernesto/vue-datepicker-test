<template>
  <div id="app">

    <div class='checker'>
      <input type='checkbox' id='show-v-date-picker' v-model='showVDatePicker'/>
      <label for='show-v-date-picker'>Show v-date-picker test</label>
    </div>
    <v-cal-date-picker-test v-show='showVDatePicker'/>

    <div class='checker'>
      <input type='checkbox' id='show-date-pick' v-model='showDatePick'/>
      <label for='show-date-pick'>Show vue-date-pick test</label>
    </div>
    <date-pick-test v-show='showDatePick'/>

    <div class='checker'>
      <input type='checkbox' id='show-vue2-datepicker' v-model='showVue2Datepicker'/>
      <label for='show-vue2-datepicker'>Show vue2-datepicker test</label>
    </div>
    <vue2-datepicker-test v-show='showVue2Datepicker'/>

    <p class='dummy-text'>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras sit amet leo hendrerit,
      convallis lectus quis, aliquam ex. Aenean eleifend
    </p>
  </div>
</template>

<script>
import VCalDatePickerTest from './components/VCalDatePickerTest.vue';
import DatePickTest from './components/DatePickTest.vue';
import Vue2DatepickerTest from './components/Vue2DatepickerTest.vue';

export default {
  name: 'App',
  components: {
    VCalDatePickerTest,
    DatePickTest,
    Vue2DatepickerTest,
  },
  data() {
    return {
      showVDatePicker: false,
      showDatePick: false,
      showVue2Datepicker: false,
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
