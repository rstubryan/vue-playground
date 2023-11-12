<script setup>
import EventCard from '@/components/EventCard.vue'
import { ref } from 'vue'

const events = ref([
  {
    id: 1,
    title: 'Vue.js Global Summit',
    date: 'September 30 - October 1, 2021',
    location: 'Online',
    time: '9:00 AM - 1:00 PM'
  },
  {
    id: 2,
    title: 'Vue.js Amsterdam',
    date: 'February 10 - 12, 2022',
    location: 'Amsterdam, Netherlands',
    time: '9:00 AM - 1:00 PM'
  },
  {
    id: 3,
    title: 'VueConf US',
    date: 'March 2 - 4, 2022',
    location: 'Austin, Texas',
    time: '9:00 AM - 1:00 PM'
  }
])
</script>

<template>
  <div>
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>
