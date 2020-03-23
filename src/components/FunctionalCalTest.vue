<template>
  <div>
    <functional-calendar
      v-model='calendarData'
      :configs='calendarConfigs'
    />
  </div>
</template>

<script>
import { FunctionalCalendar } from 'vue-functional-calendar';

export default {
  name: 'FunctionalCalTest',
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
