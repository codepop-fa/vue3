<template>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from '@/components/EventCard.vue'

export default {
  name: 'Home',
  components: {
    EventCard
  },
  data() {
    return {
      events: [
        {
          id: 5928101,
          category: 'کوهنوردی',
          title: 'صخره نوردی',
          description: 'یک صخره نوردی به یادماندنی را با ما تجربه کنید.',
          location: 'قله دماوند',
          date: '25/05/1400',
          time: '12:00',
          organizer: 'مجید بهره مند'
        },
        {
          id: 4582797,
          category: 'طبیعت',
          title: 'درختکاری',
          description: 'با کاشت یک نهال به جامعه ما بپیوندید.',
          location: 'بوستان سبز',
          date: '22/02/1400',
          time: '10:00',
          organizer: 'سینا مهران پور'
        },
        {
          id: 8419988,
          category: 'محیط زیست',
          title: 'پاکسازی ساحل',
          description: 'به جمع آوری زباله ها در کنار ساحل کمک کنید.',
          location: 'پارک ساحلی',
          date: '15/01/1400',
          time: '11:00',
          organizer: 'سعید آذری'
        }
      ]
    }
  }
}
</script>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
