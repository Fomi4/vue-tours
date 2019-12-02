<template lang="html">
  <div>
    <h1>Hello world</h1>

    <div v-if="cardInfo.length" class="tours">
      <div v-for="tour in cardInfo" :key="tour.date" class="tours_item">
        <Tour
          :destination="tour.destination"
          :date="tour.date"
          :img="tour.img"
          :description="tour.description"
        />
      </div>
    </div>
  </div>
</template>

<script>

import Tour from './Tours/Tour';

export default {
  name: 'Tours',
  components: {
    Tour
  },
  data: () => ({
    cardInfo: [
      {
        destination: 'Majorca',
        date: '05/07/2020',
        img: 'https://www.votpusk.ru/country/ctimages/new/es11.jpg',
        description: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit.'
      },
      {
        destination: 'Cyprus',
        date: '14/08/2020',
        img: 'https://iqdecision.com/wp-content/uploads/2018/11/1-69.jpg',
        description: 'Veniam deleniti reiciendis quis inventore nisi voluptatibus.'
      },
      {
        destination: 'Thailand',
        date: '31/12/2020',
        img: 'http://odominicane.com/wp-content/uploads/2014/10/of_Thailand.jpg',
        description: 'quo quibusdam ut vel vero quaerat magnam, libero dolorum tempore.'
      },
      {
        destination: 'Bali',
        date: '25/02/2020',
        img: 'https://zelenyimir.ru/wp-content/uploads/2018/02/otdyih-na-ostrove-bali-v-indonezii-1.jpg',
        description: 'harum consectetur voluptas iste? Labore.'
      }
    ]
  })
}
</script>

<style lang="css" scoped>

.tours {
  display: flex;
}

.tours_item {
  border: 1px solid #ddd;
}

</style>
