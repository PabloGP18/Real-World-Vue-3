<script setup>
import { ref } from 'vue'
import EventCard from '@/components/EventCard.vue'

const events = ref([
  {
    id: 5928101,
    category: 'animal welfare',
    title: 'Cat Adoption Day',
    description: 'Find your new feline friend at this event.',
    location: 'Meow town',
    date: 'January 28, 2022',
    time: '12:00',
    petsAllowed: true,
    organizer: 'Kay Laydee',
  },
  {
    id: 5928101,
    category: 'animal welfare',
    title: 'Cat Adoption Day',
    description: 'Find your new feline friend at this event.',
    location: 'Meow town',
    date: 'January 28, 2023',
    time: '12:00',
    petsAllowed: true,
    organizer: 'Kay Laydee',
  },
  {
    id: 5928101,
    category: 'animal welfare',
    title: 'Cat Adoption Day',
    description: 'Find your new feline friend at this event.',
    location: 'Meow town',
    date: 'January 28, 2024',
    time: '12:00',
    petsAllowed: true,
    organizer: 'Kay Laydee',
  },
])
</script>
<template>
  <h1>Events For Good</h1>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
