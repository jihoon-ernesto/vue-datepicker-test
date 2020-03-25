<template>
  <div>
    <date-picker
      range
      range-separator=" - "
      :confirm="true"
      v-model="dateRange"
      ></date-picker>
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

<style lang="scss">
$today-color: orange;

@import '~vue2-datepicker/scss/index.scss';
</style>
