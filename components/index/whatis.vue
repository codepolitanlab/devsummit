<template>
  <div>
    <div class="bg-banner" style="padding: 60px 0px 80px">
      <b-jumbotron bg-variant="transparent" class="container">
        <h1 class="banner-text mx-auto mb-0">
          WHAT IS DEV SUMMIT?
        </h1>
        <hr class="mx-auto short-hr">
        <p class="text-banner mx-auto">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
      </b-jumbotron>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.banner-text {
  width: 855px;
  height: 53px;

  font-family: Rubik;
  font-style: normal;
  font-weight: bold;
  font-size: 45px;
  line-height: 53px;
  text-align: center;
  /* identical to box height */

  color: #FFFFFF;
}
.bg-banner {
  background-image: url('static/img/banner.jpg');
  background-position: 50%;
  height: 570px;
  background-repeat: no-repeat;
  position: relative;
  background-size: cover;
  color: #181818;
}
.text-banner {
  width: 80%;
  height: 181px;

  font-family: Lato;
  font-style: normal;
  font-weight: normal;
  font-size: 25px;
  line-height: 35px;
  /* or 140% */

  text-align: center;

  color: #FFFFFF;
}

.button-started {
  width: 229px;
  height: 55px;

  background: #F79031;
  border-radius: 10px;
}
@media (max-width:767px) {
  .bg-banner {
    /* background-image: url('~assets/banner mobile.jpg'); */
    background-position: 50%;
  }
  .banner-text {
    width: 100%;
    height: 60px;

    font-family: Rubik;
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 118px;
    /* identical to box height */
    align-content: center;

    color: #FFFFFF;
  }
  .text-banner {
    width: 80%;
    height: 181px;

    font-family: Lato;
    font-style: normal;
    font-weight: normal;
    font-size: 15px;
    line-height: 20px;
    /* or 140% */

    text-align: center;

    color: #FFFFFF;
  }
}
.button-started:hover {
  background-color: #B24A00;
}
</style>
