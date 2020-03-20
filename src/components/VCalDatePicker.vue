<template>
  <div>
    <v-date-picker
      v-model='dateRange'
      mode='range'
      :masks='masks'
      />
  </div>
</template>

<script>
import DatePicker from 'v-calendar/lib/components/date-picker.umd'

export default {
  name: 'VCalDatePicker',
  props: {
    initDate: String
  },
  components: {
    'v-date-picker': DatePicker,
  },
  data() {
    return {
      dateRange: {
        start: new Date(2020, 2, 19),
        end: new Date(2020, 3, 5),
      },
      masks: {
        input: ['YYYY-MM-DD'],
      },
    };
  }
}
</script>

<style scoped>
</style>
