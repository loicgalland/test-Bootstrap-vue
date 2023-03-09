<template>
  <div class="container">
    <NavBar />
  </div>
  <div class="container">
    <div class="row">
        <CardsHotels 
          v-for="hotel in hotels"
          :title="hotel.title"
          :description="hotel.description"
          :id="hotel.id"
          :image="hotel.image"
          :key="hotel.title"/>
    </div>
  </div>
  
</template>

<script>
import CardsHotels from './components/cards.vue'
import NavBar from './components/navbar.vue'

export default {
  name: 'App',
  components: {
    CardsHotels,
    NavBar
  },
  data() {
  return {
          adress: "15 rue du générale de Gaulle 71200 Charolles",
          hotels: [
          {id: 1, title: "Hotel F1", description: "Un peu miteux mais mieux que rien !", image: "https://picsum.photos/200/100"},
          {id: 2, title: "Ibis", description: "Un lit confortable.", image: "https://picsum.photos/200/100"},
          {id: 3, title: "Palacio", description: "Un vrai palace, tout est fait pour vous rendre heureux !", image: "https://picsum.photos/200/100"},
          {id: 4, title: "La Cabane", description: "Une expérience insolite, dormir dans un arbre.", image: "https://picsum.photos/200/100"},
          {id: 5, title: "Grotte", description: "N'ayez pas peur de dormir dans un trou !", image: "https://picsum.photos/200/100"},
          {id: 6, title: "Jungle", description: "Des plantes, des plantes et des plantes.", image: "https://picsum.photos/200/100"}
          ]
      }
  }
}

</script>

<style lang="scss">

</style>
