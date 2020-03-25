<template>
  <div>
    <date-picker v-model="dateRange" range></date-picker>
  </div>
</template>

<script>
import DatePicker from 'vue2-datepicker';
import 'vue2-datepicker/index.css';

export default {
  name: 'Vue2DatepickerTest',
  props: {
  },
  components: {
    DatePicker,
  },
  data() {
    return {
      dateRange: null,
    };
  }
}
</script>

<style>
</style>
