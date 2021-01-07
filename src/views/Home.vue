<template>
  <h1>Events for Good</h1>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event"/>
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "Home",
  components: {
    EventCard
  },
  data() {
    return {
      events: [
        {
        id: 1232452,
        category: 'animal welfare',
        title: 'Chi adoption day',
        description: 'Get a chihuahua into your home',
        location: 'Woof Park',
        date: 'January 10, 2021',
        time: '5:00',
        petsAllowed: true,
        organizer: 'Dulce'
      },
      {
        id: 123245332,
        category: 'animal welfare',
        title: 'Chi adoption day',
        description: 'Get a chihuahua into your home',
        location: 'Woof Park',
        date: 'January 10, 2021',
        time: '5:00',
        petsAllowed: true,
        organizer: 'Dulce'
      },
      {
        id: 123222452,
        category: 'animal welfare',
        title: 'Chi adoption day',
        description: 'Get a chihuahua into your home',
        location: 'Woof Park',
        date: 'January 10, 2021',
        time: '5:00',
        petsAllowed: true,
        organizer: 'Dulce'
      }
      ]
    }
  }
};
</script>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>