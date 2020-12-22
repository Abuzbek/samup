<template>
  <v-app>
    <v-app-bar app color="white" height="120px">
      <div style="width:100%;" class="d-flex justify-center align-center">
        <v-btn tag="a" style="font-size:20px" v-for="n in buttonLeft" :key="n.name" depressed color="transparent">
          {{ n.name }}
        </v-btn>
          <img
            alt="star Logo"
            class="shrink mx-8 logoHeader d-none_Logomd btnSrc"
            style="flex: 0 0 auto; "
            :src="require('./assets/logo yellow 1.png')"
          >
        <v-btn tag="a" :style="`font-size:20px; font-weight:${n.weight};`" v-for="n in buttonRight" :key="n.name" depressed color="transparent">
          {{ n.name }}
        </v-btn>
      </div>
    </v-app-bar>
    <v-main>
      <Header/>
      <About/>
      <services/>
      <Portfolio/>
      <Client/>
    </v-main>
  </v-app>
</template>

<script>
import Header from './components/header'
import About from './components/about'
import services from './components/services'
import Portfolio from './components/portfolio'
import Client from './components/Client'

export default {
  name: "App",

  components: {Header,About,services,Portfolio,Client},

  data: () => ({
    buttonLeft:[
      {
        name:'Biz haqimizda'
      },
      {
        name:'Xizmatlarimiz'
      },
      {
        name:'Portfolio'
      },
    ],
    buttonRight:[
      {
        name:'Mijozlarimiz'
      },
      {
        name:'Kontaktlarimiz'
      },
      {
        name:'+99898 190 60 70',
        weight:'600'
      },
    ]
  }),
};
</script>
<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;600;700;800&display=swap');

</style>
