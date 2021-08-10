<template>
  <section class="space--xs">
    <p class="title-text">
      MEET THE MENTORS
    </p>
    <div class="mt-5 container-fluid mentor-div">
      <b-row class="justify-content-center">
        <cardmentor :mentor="'Alexander Makarov'" :img="'/img/alexander.jfif'" :job="'Lead Developer of Yii Framework'" />
        <cardmentor :mentor="'Kresna Galuh'" :img="'/img/kresna.png'" :job="'CEO  of Codepolitan'" />
        <cardmentor :mentor="'Taufan Aditya'" :img="'/img/taufan.jpg'" :job="'CEO of Refactory'" />
        <cardmentor :mentor="'Puja Pramudya'" :img="'/img/puja.jpeg'" :job="'Co-founder of Radya Labs'" />
        <cardmentor :mentor="'Mulia Nasution'" :img="'/img/mulia.jpg'" :job="'Co-founder of Refactory Indonesia'" />
        <cardmentor :mentor="'Oscar Darmawan'" :img="'/img/oscar.jpeg'" :job="'CEO at Bitcoin Indonesia'" />
        <cardmentor :mentor="'Muhammad Yulianto'" :img="'/img/yulianto.jpg'" :job="'Tech Lead Engineer at Importir.org'" />
      </b-row>
    </div>
    <!-- <div class="d-flex justify-content-center">
      <nuxt-link to="/mentor">
        <b-button class="button-mentor d-flex align-items-center">
          <p class="mx-auto">
            SEE ALL THE MENTORS
          </p>
        </b-button>
      </nuxt-link>
    </div> -->
  </section>
</template>

<script>
import Cardmentor from '../cardmentor.vue'
export default {
  components: { Cardmentor }
}
</script>

<style scoped>
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
