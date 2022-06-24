<template>
  <div class="week-row">
    <day-week v-for="day in 7" :key="day"></day-week>
  </div>
</template>

<script>
import DayWeek from '@/components/calendar/DayWeek'

export default {
  name: 'WeekRow',

  components: {
    DayWeek
  }
}
</script>

<style lang="scss" scoped>
@import "@/assets/style/var.scss";
.week-row {
  flex: auto;
  display: grid;
  grid-template-columns: repeat(7, 1fr);
  background-color: $borders-color;
  border-left: 1px solid $borders-color;
}

.week-row:first-child {
  border-top: 1px solid $borders-color;
}
</style>
