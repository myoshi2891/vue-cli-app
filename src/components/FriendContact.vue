<template>
  <li>
    <h2>{{ name }} {{ friendIsFavorite === '1' ? '(Favorite)' : '' }}</h2>
    <button @click="toggleDetails">{{  detailsAreVisible ? 'Hide' : 'Show'  }} Details</button>    
    <button @click="toggleFavorite">Toggle Favorite</button>    
    <ul v-if="detailsAreVisible">
      <li><strong>Phone:</strong> {{ phoneNumber }}</li>
      <li><strong>Email:</strong> {{ emailAddress }}</li>
    </ul>
  </li>
</template>

<script>
export default {
  props: [
    'name',
    'phoneNumber',
    'emailAddress',
    'isFavorite'
  ],
  data() {
    return {
      detailsAreVisible: false,
      friend: {
          id: 'manual',
          name: 'Manual Lorenz',
          phone: '0197 2894 2689',
          email: 'manual@example.com'
      },
      friendIsFavorite: this.isFavorite
    }
  },
  methods: {
    toggleDetails() {
      this.detailsAreVisible = !this.detailsAreVisible;
    },
    toggleFavorite() {
      if (this.friendIsFavorite === '1') {
        this.friendIsFavorite = '0'
      } else {
        this.friendIsFavorite = '1'
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<!-- <style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style> -->
