<template>
  <div>
    <jumbotron />
    <statistic />
    <whatis />
    <meetmentor />
  </div>
</template>

<script>
import jumbotron from '../components/index/jumbotron.vue'
import Meetmentor from '../components/index/meetmentor.vue'
import Statistic from '../components/index/statistic.vue'
import Whatis from '../components/index/whatis.vue'
export default {
  components: { jumbotron, Statistic, Whatis, Meetmentor }
}
</script>
