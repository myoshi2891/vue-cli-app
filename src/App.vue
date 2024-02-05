<template>
  <section>
    <h2>My Friends</h2>

    <ul>
      <li></li>
    </ul>
  </section>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

// export default {
//   name: 'App',
//   components: {
//     HelloWorld
//   }
// }
export default {
  data() {
    return {
      friends: [
        {
          id: 'manual',
          name: 'Manual Lorenz',
          phone: '0197 2894 2689',
          email: 'manual@example.com'
        },
        {
          id: 'julie',
          name: 'Julie Jones',
          phone: '0197 8784 2689',
          email: 'julie@example.com'
        },

      ]
    }
  }
}
</script>

<!-- <style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style> -->
