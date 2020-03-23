<template>
  <div>
    <vue-ctk-date-time-picker
      v-model='date'
      :range='true'
      :only-date='true'
      format='YYYY-MM-DD'
      formatted='L'
      outputFormat='YYYY-MM-DD'
    />
  </div>
</template>

<script>
import VueCtkDateTimePicker from 'vue-ctk-date-time-picker';
import 'vue-ctk-date-time-picker/dist/vue-ctk-date-time-picker.css';

export default {
  name: 'CtkDatetimePickerTest',
  props: {
  },
  components: {
    VueCtkDateTimePicker,
  },
  data() {
    return {
      date: {
        start: '2020-03-19',
        end: '2020-04-22',
      }
    };
  }
}
</script>

<style scoped>
</style>
