<template>
    <a id="ch2" href="" @click.prevent="$emit('changePicture',cardimage)" class="d-flex flex-column p-3 rounded nav-link" style="background-color: white;">
        <img :src="require('./img/' + cardimage + '.png')" alt="">
        <div class="pt-3 nav-link text-dark"><b>{{ cardtitle }}</b></div>
        <div class="nav-link text-dark">{{ cardprice }}</div>
        <!-- <p>{{eea}}</p> -->
    </a>
</template>
<script>
export default {
  name: 'CardS',
  // data(){
  //   return{
  //     aLink: "jjj",
  //     eea: "jjj"
  //   }
  // },
  props: [
    "cardimage","cardprice","cardtitle"
  ]
}
</script>