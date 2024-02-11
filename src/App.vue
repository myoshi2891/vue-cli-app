<template>
  <ul></ul>
</template>

<script>
export default {
  data() {
    return {
      storedResources: [
        {
          id: 'official-guide', title: 'Official Guide', description: 'The official Vue.js documentation',
          link: 'https://vue.js.org'
        },
        {
          id: 'google', title: 'Google', description: 'Learn to google',
          link: 'https://google.org'
        },
        ]
      }
    }
  } 
</script>

<style>
html {
  font-family: sans-serif;
}

body {
  margin: 0;
}
</style>