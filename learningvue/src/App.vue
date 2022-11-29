<template>
  <div id="app">
    <Header></Header>
    <Nav></Nav>
    <Main :cardimage="imgLink"></Main>
    <MainComponent @changePicture="changePicture"></MainComponent>
    <!-- <Card nama="nana" harga="haha"></Card> -->
    <Footer></Footer>

    
    
  </div>
</template>

<script>

import Header from './components/HeaderA.vue'
import Nav from './components/NavU.vue'
import Main from './components/MainP.vue'
import MainComponent from './components/MainD.vue'
// import MainComponent from './components/MainD.vue'
import Footer from './components/FooterM.vue'
// import Card from './components/CardS.vue'

export default {
  name: 'App',
  data: function(){
    return{
      nama : "Kodehive",
      anggota : ["bayu","eka","Rangga"],
      quantity : 5,
      barang : ["Kursi 1,Kursi 2,Kursi 3,Kursi 4"],
      harga : [1,2,3,4],
      imgLink : "chair"
    }
  },
  methods: {
    gantiNama : function(){
      this.nama = "gua"
    },
    changePicture : function(imgLink){
      this.imgLink = imgLink
    },
  gantiQuantity : function(){
      this.quantity++
    }
  },
  computed: {
    totalBelanja : function(){
      return this.quantity * 10000
    }
  },
  components: {
    // HelloWorld
    Header,
    Nav,
    Main,
    MainComponent,
    Footer,
    // Card
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}
</style>
