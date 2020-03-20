<template>
  <div>
    <FunctionalCalendar
      v-model='calendarData'
      :configs='calendarConfigs'
    ></FunctionalCalendar>
  </div>
</template>

<script>
import { FunctionalCalendar } from 'vue-functional-calendar';

export default {
  name: 'FunctionalCal',
  props: {
  },
  components: {
    FunctionalCalendar,
  },
  data() {
    return {
      calendarData: {},
      calendarConfigs: {
        isModal: true,
        isDateRange: true,
        changeYearFunction: true,
        changeMonthFunction: true,
      },
    };
  }
}
</script>

<style scoped>
</style>
