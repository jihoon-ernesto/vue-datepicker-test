<template>
  <div>
    <date-pick id='start-date' class='date-pick'
      v-model='startDate'
      :startWeekOnSunday='true'
      :selectableYearRange='10'
    />
    <date-pick id='end-date' class='date-pick'
      v-model='endDate'
      :startWeekOnSunday='true'
      :selectableYearRange='5'
    />
  </div>
</template>

<script>
import DatePick from 'vue-date-pick';
import 'vue-date-pick/dist/vueDatePick.css';

export default {
  name: 'DatePickTest',
  props: {
  },
  components: {
    DatePick,
  },
  data() {
    return {
      startDate: '2020-03-20',
      endDate: '2020-03-31',
    };
  },
  watch: {
    startDate(date) {
      console.log(`new startDate: ${date}`);
    },
    endDate(date) {
      console.log(`new endDate: ${date}`);
    },
  },
}
</script>

<style lang="scss">
$themeColor: #cc99cd;

/* ref) https://dbrekalo.github.io/vue-date-pick/customizing-appearance.html */
.vdpArrowPrev:after {
  border-right-color: $themeColor;
}

.vdpArrowNext:after {
  border-left-color: $themeColor;
}

.vdpCell.selectable:hover .vdpCellContent,
.vdpCell.selected .vdpCellContent {
  background: $themeColor;
}

.vdpCell.today {
  color: $themeColor;
}

.vdpTimeUnit > input:hover,
.vdpTimeUnit > input:focus {
  border-bottom-color: $themeColor;
}

/*
  the styles below are from:
  https://dbrekalo.github.io/vue-date-pick/examples.html#calendar-widget
*/
.date-pick {
  margin:0 0 20px;
}
.date-pick > input {
  font-size:16px;
  display:block;
  width:100%;
  box-sizing:border-box;
  padding:15px;
  padding-right:40px;
  -webkit-appearance:none;
  -moz-appearance:none;
  appearance:none;
  border-radius:4px;
  background:transparent;
  border:1px solid #e0e0e0;
  box-shadow:0 .1em .3em rgba(0,0,0,.05);
  outline:0
}

</style>
