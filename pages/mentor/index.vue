<template>
  <div>
    <top />
    <text-area />
    <keynote />
    <case-study />
    <workshop />
  </div>
</template>

<script>
import CaseStudy from '@/components/mentor/case-study.vue'
import Keynote from '@/components/mentor/keynote.vue'
import textArea from '@/components/mentor/text-area.vue'
import top from '@/components/mentor/top.vue'
import Workshop from '@/components/mentor/workshop.vue'
export default {
  components: { top, textArea, Keynote, CaseStudy, Workshop }
}
</script>

<style>

</style>
