<template>
  <section class="space--xs">
    <p class="title-text">
      MEET THE MENTORS
    </p>
    <div class="mt-5 container-fluid mentor-div">
      <b-row cols="2" cols-md="4">
        <cardmentor :mentor="'ABCD'" :img="'https://picsum.photos/400/400/?image=20'" :job="'head of anime industry'" />
        <cardmentor :mentor="'efgh'" :img="'https://picsum.photos/400/400/?image=20'" :job="'head of anime industry'" />
        <cardmentor :mentor="'ijkl'" :img="'https://picsum.photos/400/400/?image=20'" :job="'head of anime industry'" />
        <cardmentor :mentor="'mnop'" :img="'https://picsum.photos/400/400/?image=20'" :job="'head of anime industry'" />
      </b-row>
    </div>
    <div class="d-flex justify-content-center">
      <nuxt-link to="/mentor">
        <b-button class="button-mentor d-flex align-items-center">
          <p class="mx-auto">
            SEE ALL THE MENTORS
          </p>
        </b-button>
      </nuxt-link>
    </div>
  </section>
</template>

<script>
import Cardmentor from '../cardmentor.vue'
export default {
  components: { Cardmentor }
}
</script>

<style scope
Cardmentord>
.title-text {
  height: 53px;
  top: 1525px;

  font-family: Rubik;
  font-style: normal;
  font-weight: bold;
  font-size: 45px;
  line-height: 53px;
  text-align: center;

  color: #303956;
}
.button-mentor {
  width: 277px;
  height: 30px;

  font-family: Rubik;
  font-style: normal;
  font-weight: 500;
  font-size: 25px;
  line-height: 30px;
  /* identical to box height */

  color: #F79031;
  background-color: transparent;
  border-color: #F79031;
}
.button-mentor:hover {
  background-color: #f79021;
}
@media (min-width:767px) {
  .mentor-div {
    padding-left: 100px;
    padding-right: 100px;
  }
}
</style>
