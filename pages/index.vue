<template>
  <div>
    <jumbotron />
    <statistic />
    <whatis />
    <meetmentor />
    <moments />
    <partner />
  </div>
</template>

<script>
import jumbotron from '../components/index/jumbotron.vue'
import Meetmentor from '../components/index/meetmentor.vue'
import Moments from '../components/index/moments.vue'
import Partner from '../components/index/partner.vue'
import Statistic from '../components/index/statistic.vue'
import Whatis from '../components/index/whatis.vue'
export default {
  components: { jumbotron, Statistic, Whatis, Meetmentor, Moments, Partner }
}
</script>
