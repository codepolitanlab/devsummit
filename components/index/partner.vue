<template>
  <section class="space--xs text-center type--uppercase pt-0">
    <b-container>
      <div class="text-center mb--2">
        <div>
          <p class="partner-title">
            THE PARTNERS
          </p>
        </div>
      </div>
      <b-container class="d-md-flex justify-content-md-center mt-5 mt-md-0">
        <b-row cols="2" cols-md="5" class="d-md-flex justify-content-md-center">
          <div class="d-flex align-items-center mt-5 mt-md-0">
            <b-img-lazy class="mx-auto" height="110" src="/img/partner/KEMNAKER.png" />
          </div>
          <div class="d-flex align-items-center mt-5 mt-md-0">
            <b-img-lazy class="mx-auto" height="110" src="/img/partner/here.png" />
          </div>
          <div class="d-flex align-items-center mt-5 mt-md-0">
            <b-img-lazy class="mx-auto" src="/img/partner/udemy.png" />
          </div>
          <div class="d-flex align-items-center mt-5 mt-md-0">
            <b-img-lazy class="mx-auto" width="156" height="110" src="/img/partner/samsung.png" />
          </div>
        </b-row>
      </b-container>
    </b-container>
  </section>
</template>

<script>
export default {

}
</script>

<style scoped>
.w-80 {
  width: 80vw;
  border-top: 0.5px solid #d3d3d3;
}
.partner-logo {
  padding-top: 50px;
}

.partner-logo img {
  margin-left: 25px;
  margin-right: 25px;
  margin-bottom: 25px;
}
.partner-title {
  height: 53px;

  font-family: Rubik;
  font-style: normal;
  font-weight: bold;
  font-size: 45px;
  line-height: 53px;

  color: #303956;
}
</style>
