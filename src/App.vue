<template>
  <div class="main-wrapper">
    <the-header />
    <app-calendar />
  </div>
</template>

<script>
import TheHeader from '@/components/TheHeader'
import AppCalendar from '@/components/calendar/AppCalendar'

export default {
  name: 'App',
  components: {
    TheHeader,
    AppCalendar
  }
}
</script>

<style lang="scss">
#app {
  height: 100%;
}
</style>

<style lang="scss" scoped>
.main-wrapper {
  display: flex;
  flex-direction: column;
  height: 100%;
}
</style>
