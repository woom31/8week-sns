<template>
  <FeedWrapper/>
</template>

<script>
import FeedWrapper from './components/feed/FeedWrapper.vue'

export default {
  name: 'App',
  components: {
    FeedWrapper
  }
}
</script>

<style>
@import "./css/feed.css";
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */

</style>
