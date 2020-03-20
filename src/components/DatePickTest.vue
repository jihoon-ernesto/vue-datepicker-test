<template>
  <div>
    <p>DatePick test</p>
    <date-pick
      v-model='date'
      :startWeekOnSunday='true'
    ></date-pick>
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
      date: '2020-03-20',
    };
  },
}
</script>

<style>
.vdpArrowPrev:after {
    border-right-color: #cc99cd;
}

.vdpArrowNext:after {
    border-left-color: #cc99cd;
}

.vdpCell.selectable:hover .vdpCellContent,
.vdpCell.selected .vdpCellContent {
    /* background: #cc99cd; */
    background: lightgreen;
}

.vdpCell.today {
    color: #cc99cd;
}

.vdpTimeUnit > input:hover,
.vdpTimeUnit > input:focus {
    border-bottom-color: #cc99cd;
}

</style>
