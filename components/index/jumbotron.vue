<template>
  <div>
    <div class="bg-jumbotron" style="padding: 60px 0px 80px">
      <b-jumbotron bg-variant="transparent" class="container">
        <h1 class="jumbotron-text mx-auto mb-0">
          DEV SUMMIT 2022
        </h1>
        <hr class="mx-auto short-hr">
        <h5 class="text-jumbotron mx-auto">
          Conference | Expo | Hackathon
        </h5>
        <div class="d-flex justify-content-center">
          <b-button class="button-started">
            GET STARTED
          </b-button>
        </div>
      </b-jumbotron>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.jumbotron-text {
  width: 855px;
  height: 119px;
  top: 233px;

  font-family: Rubik;
  font-style: normal;
  font-weight: normal;
  font-size: 100px;
  line-height: 118px;
  /* identical to box height */

  color: #FFFFFF;
}
.short-hr {
  width: 95px;
  height: 0px;
  border-bottom: 3px solid #99D9D6;
}
.bg-jumbotron {
  background-image: url('static/img/jumbotron.jpg');
  background-position: 50%;
  height: 570px;
  background-repeat: no-repeat;
  position: relative;
  background-size: cover;
  color: #181818;
}
.text-jumbotron {
  height: 42px;

  font-family: Lato;
  font-style: normal;
  font-weight: 200;
  font-size: 35px;
  line-height: 42px;
  /* identical to box height */

  text-align: center;

  color: #FFFFFF;

  /* border: 1px solid #FFFFFF; */
}

.button-started {
  width: 229px;
  height: 55px;

  background: #F79031;
  border-radius: 10px;
}
@media (max-width:767px) {
  .bg-jumbotron {
    /* background-image: url('~assets/banner mobile.jpg'); */
    background-position: 50%;
  }
  .jumbotron-text {
    width: 100%;
    height: 60px;

    font-family: Rubik;
    font-style: normal;
    font-weight: normal;
    font-size: 38px;
    line-height: 118px;
    /* identical to box height */
    align-content: center;

    color: #FFFFFF;
  }
}
.button-started:hover {
  background-color: #B24A00;
}
</style>
