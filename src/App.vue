<script>
import Textbind from './components/Textbind.vue'
export default {
  components: {
    components: {
      Textbind,
    },
  },
  data() {
      return {
        bind_url : 'http://www.daum.net',
        bind_a : {
          bind_url : 'http://www.daum.net',
          domain_name : 'daum',
        }, 
      }
    }
}
</script>

<template>
  <img src="https://placeimg.com/100/100/any" alt="image size 100-100">
  <h2 id="title">Hello World</h2>
  <a v-bind:href="bind_a.bind_url">{{bind_a.domain_name}}</a>
  <!-- <Textbind /> -->
</template>

<style scoped>
#title {
  color: blueviolet;
  text-align: center;
}
</style>