<template>
  <div class="calendar-block">
    <week-row v-for="item in 6" :key="item"></week-row>
  </div>
</template>

<script>
import WeekRow from '@/components/calendar/WeekRow'

export default {
  name: 'AppCalendar',

  components: {
    WeekRow
  }
}
</script>

<style lang="scss" scoped>
.calendar-block {
  display: flex;
  flex-direction: column;
  height: 100%;
  padding: 20px;
}
</style>
