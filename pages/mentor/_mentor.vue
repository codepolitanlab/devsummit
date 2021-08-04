<template>
  <div>
    <top />
    <text-area />
    <detail />
  </div>
</template>

<script>
import textArea from '@/components/detail/text-area.vue'
import top from '@/components/detail/top.vue'
import Detail from '../../components/detail/detail.vue'
export default {
  components: { top, textArea, Detail },
  data () {
    return {
      link: this.$route.params.mentor
    }
  }
}
</script>

<style>

</style>
