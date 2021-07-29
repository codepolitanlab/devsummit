<template>
  <b-col>
    <b-card img-top style="border: none; border-radius: 20px;" :img-src="img">
      <b-card-title class="title-card">
        {{ mentor }}
      </b-card-title>
      <b-card-text class="sub-title-card">
        {{ job }}
      </b-card-text>
    </b-card>
  </b-col>
</template>

<script>
export default {
  props: ['img', 'mentor', 'job']
}
</script>

<style scoped>
img {
  background: linear-gradient(0deg, rgba(247, 147, 50, 0.25), rgba(247, 147, 50, 0.25));
  border-top-left-radius: 20px !important;
  border-top-right-radius: 20px !important;
  margin-bottom: 0;
}
.card-body {
  height: 150px;
  position: relative;
  top: -50px;
  background: #F79231;
  border-radius: 0px 0px 20px 20px;
}
.title-card {
  font-family: Rubik;
  font-style: normal;
  font-weight: bold;
  font-size: 35px;
  line-height: 45px;
  color: #FFFFFF;
}
.sub-title-card {
  color: #B75A00;
}
</style>
