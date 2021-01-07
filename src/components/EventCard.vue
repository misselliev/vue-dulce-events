<template>
  <div class="event-card">
    <!-- Display data -->
    <span>@ {{ event.time  }} on {{event.date}} </span>
    <h4>{{ event.title }}</h4>
    
  </div>
</template>

<script>
export default {
  name: "EventCard",
  props: {
    events: Object
  },
  data() {
    return {
      event: {
        id: 1232452,
        category: 'animal welfare',
        title: 'Chi adoption day',
        description: 'Get a chihuahua into your home',
        location: 'Woof Park',
        date: 'January 10, 2021',
        time: '5:00',
        petsAllowed: true,
        organizer: 'Dulce'
      }
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.event-card {
  padding: 20px;
  width: 250px;
  cursor: pointer;
  border: 1px solid #39495c;
  margin-bottom: 18px;
}

.event-card:hover {
  transform: scale(1.01);
  box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2);
}
</style>
