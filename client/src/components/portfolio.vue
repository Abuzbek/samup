<template>
  <section class="portfolio">
    <v-container fluid>
      <v-row>
        <v-col cols="12" md="2" >
          <img class="d-block_sm" :src="require('../assets/img/Group 53.jpg')" alt="" />
          <img class="d-block_sm" :src="require('../assets/img/Group 54.jpg')" alt="" />
          <img class="d-block_sm" :src="require('../assets/img/Group 55.jpg')" alt="" />
          <img class="d-block_sm" :src="require('../assets/img/Group 56.jpg')" alt="" />
        </v-col>
        <v-col cols="12" md="8">
          <v-row style="height: 100%;">
            <v-col cols="12">
              <v-row>
                <v-col
                  cols="12"
                  sm="7"
                  class="ma-auto d-flex justify-center align-center flex-column"
                >
                  <h3>Zamonaviy upakovkaga buyurtma bering!</h3>
                  <p>
                    Biz bilan bog’laning va o'z mahsulotingiz uchun chiroyli,
                    zamonaviy dizayn va upakovkaga ega bo'ling.
                  </p>
                  <v-btn class="btnDep" tag="a" depressed color="#FEB11B">
                    Buyurtma berish
                  </v-btn>
                </v-col>
              </v-row>
            </v-col>
            <v-col cols="6" sm="4" class="d-flex justify-center flex-column">
              <img :src="require('../assets/img/Group 57.jpg')" alt="" />
              <img :src="require('../assets/img/Group 58.jpg')" alt="" />
              <img :src="require('../assets/img/Group 59.jpg')" alt="" />
              <img :src="require('../assets/img/Group 55.jpg')" class="d-none_sm"  alt="" />
              <img :src="require('../assets/img/Group 56.jpg')" class="d-none_sm"  alt="" />
            </v-col>
            <v-col
              cols="6"
              sm="4"
              class="d-flex justify-end flex-column"
              style="transform:translateY(100px);"
            >
              <img :src="require('../assets/img/Group 60.jpg')" alt="" />
              <img :src="require('../assets/img/Group 61.jpg')" alt="" />
              <img :src="require('../assets/img/Group 62.jpg')" alt="" />
              <img :src="require('../assets/img/Group 68.jpg')" class="d-none_sm" alt="" />
              <img :src="require('../assets/img/Group 69.jpg')" class="d-none_sm" alt="" />
            </v-col>
            <v-col cols="6" sm="4" class="d-flex justify-center flex-column">
              <img :src="require('../assets/img/Group 63.jpg')" alt="" />
              <img :src="require('../assets/img/Group 64.jpg')" alt="" />
              <img :src="require('../assets/img/Group 65.jpg')" alt="" />
              <img :src="require('../assets/img/Group 66.jpg')" class="d-none_sm" alt="" />
              <img :src="require('../assets/img/Group 67.jpg')" class="d-none_sm" alt="" />
            </v-col>
          </v-row>
        </v-col>
        <v-col cols="12" md="2">
          <img class="d-block_sm" :src="require('../assets/img/Group 66.jpg')" alt="" />
          <img class="d-block_sm" :src="require('../assets/img/Group 67.jpg')" alt="" />
          <img class="d-block_sm" :src="require('../assets/img/Group 68.jpg')" alt="" />
          <img class="d-block_sm" :src="require('../assets/img/Group 69.jpg')" alt="" />
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
section{
  padding-top: 100px ;
  padding-bottom: 250px;
}
img {
  max-width: 100%;
  height: auto;
  padding: 15px 0;
}
h3 {
  font-family: "Open Sans";
  font-style: normal;
  font-weight: bold;
  font-size: 36px;
  line-height: 130%;
  text-align: center;
  color: #000000;
  padding: 0 52px;
}
p {
  font-family: "Open Sans";
  font-style: normal;
  font-weight: normal;
  font-size: 24px;
  line-height: 130%;
  text-align: center;
  color: #000000;
  padding: 0 10px;
  margin-bottom: 30px;
}
.btnDep {
  padding: 23px 62px !important;
  height: auto !important;
  font-weight: 600 !important;
  font-size: 24px !important;
}
.d-none_sm{
  display: none;
}
@media (max-width:1500px) {
  h3 {
  font-family: "Open Sans";
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 130%;
  text-align: center;
  color: #000000;
  padding: 0 52px;
}
p {
  font-family: "Open Sans";
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 130%;
  text-align: center;
  color: #000000;
  padding: 0 10px;
  margin-bottom: 30px;
}
.btnDep {
  padding: 23px 62px !important;
  height: auto !important;
  font-weight: 600 !important;
  font-size: 18px !important;
}
}
@media (max-width:959px) {
  .d-none_sm{
    display: block;
  }
  .d-block_sm{
    display: none;
  }
  h3 {
  font-family: "Open Sans";
  font-style: normal;
  font-weight: bold;
  font-size: 36px;
  line-height: 130%;
  text-align: center;
  color: #000000;
  padding: 0 52px;
}
p {
  font-family: "Open Sans";
  font-style: normal;
  font-weight: normal;
  font-size: 24px;
  line-height: 130%;
  text-align: center;
  color: #000000;
  padding: 0 10px;
  margin-bottom: 30px;
}
.btnDep {
  padding: 23px 62px !important;
  height: auto !important;
  font-weight: 600 !important;
  font-size: 24px !important;
}
}
</style>
