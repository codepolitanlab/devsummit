<template>
  <section class="space--xs">
    <div class="container">
      <h1 class="keynote-text mx-auto mb-0">
        Keynote Speaker
      </h1>
    </div>
    <div class="container section-keynote">
      <b-row cols="2" cols-md="4">
        <cardmentor :mentor="'ABCD'" :img="'https://picsum.photos/400/400/?image=20'" :job="'head of anime industry'" />
        <cardmentor :mentor="'efgh'" :img="'https://picsum.photos/400/400/?image=20'" :job="'head of anime industry'" />
        <cardmentor :mentor="'ijkl'" :img="'https://picsum.photos/400/400/?image=20'" :job="'head of anime industry'" />
      </b-row>
    </div>
  </section>
</template>

<script>
import Cardmentor from '../cardmentor.vue'
export default {
  components: { Cardmentor }
}
</script>

<style scoped>
.keynote-text {
  font-family: Rubik;
  font-style: normal;
  font-weight: normal;
  font-size: 45px;
  line-height: 53px;
  padding-left: 5px;
  color: #B75A00;
  border-left: 5px solid #F79031;;
}
.section-keynote {
  margin-top: 85px;
}
</style>
