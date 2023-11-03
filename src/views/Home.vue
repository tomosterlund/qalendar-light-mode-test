<template>
  <div class="calendar-container is-light-mode">
    <Qalendar :events="events" />
  </div>
</template>

<script lang="ts" setup>
  import { Qalendar } from "qalendar";
  import { ref } from "vue";

  const events = ref([
    {
      id: 1,
      title: 'hello',
      time: {
        start: '2023-11-03 10:00',
        end: '2023-11-03 12:00'
      }
    }
  ])
</script>

<style>
@import "qalendar/dist/style.css";

.calendar-container {
  width: 100%;
  height: 800px;
  left: 0;
}
</style>
