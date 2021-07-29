<template>
  <div class="statistic-banner">
    <div class="container text-center container-stat">
      <p class="heading-stat mb-5">
        More Than
      </p>
      <div class="d-flex justify-content-around">
        <div class="data-stat">
          <span class="text-stat">
            10
          </span>
          <br>
          <span class="sub-text-stat">
            City
          </span>
        </div>
        <div class="data-stat">
          <span class="text-stat">
            14
          </span>
          <br>
          <span class="sub-text-stat">
            Mentor
          </span>
        </div>
        <div class="data-stat">
          <span class="text-stat">
            10000+
          </span>
          <br>
          <span class="sub-text-stat">
            Attendees
          </span>
        </div>
        <div class="data-stat">
          <span class="text-stat">
            50+
          </span>
          <br>
          <span class="sub-text-stat">
            Topics
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.statistic-banner {
  width: 100%;
  height: 250px;

  background: linear-gradient(90deg, #F79031 0%, #F8A735 101.9%);
}
.container-stat {
  padding-top: 30px;
  padding-bottom: 59px;
}
.heading-stat {
  height: 41px;

  font-family: Rubik;
  font-style: normal;
  font-weight: 500;
  font-size: 35px;
  line-height: 41px;

  color: #FFFFFF;
}
.data-stat {
  height: 87px;
}
.text-stat {
  height: 42px;

  font-family: Lato;
  font-style: normal;
  font-weight: bold;
  font-size: 35px;
  line-height: 42px;
  /* identical to box height */

  text-align: center;

  color: #FFFFFF;
}
.sub-text-stat {
  height: 30px;

  font-family: Lato;
  font-style: normal;
  font-weight: normal;
  font-size: 25px;
  line-height: 30px;
  /* identical to box height */

  text-align: center;

  color: #FFFFFF;
}
</style>
