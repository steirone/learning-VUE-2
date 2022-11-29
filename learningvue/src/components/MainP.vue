<template>
    <div class="d-flex p-4">
        <div class="d-flex flex-column">
            <a href="" id="s1"><img src="./img/chair.png" style="border-radius: 25px; width: 100px;" class="p-3" alt=""></a>
            <a href="" id="s2"><img src="./img/side-1.png" style="border-radius: 25px; width: 100px;" class="p-3" alt=""></a>
            <a href="" id="s3"><img src="./img/side-2.png" style="border-radius: 25px; width: 100px;" class="p-3" alt=""></a>
            <a href="" id="s4"><img src="./img/side-3.png" style="border-radius: 25px; width: 100px;" class="p-3" alt=""></a>
            
        </div>
        <!-- <div class="d-flex">
            <img src="img/chair.png" style="width: 68%;" alt="">
        </div> -->
        <div style="width: 380px; height: 410px;">
            <img id="picu" :src="require('./img/' + cardimage + '.png')" class="p-3" style="width: 380px; height: 410px; border-radius: 25px;" alt="">
        </div>
        <div class="d-flex flex-column">
            <h1 id="namu">Chair Thatty</h1>
            <div id="haru" class="pb-3">IDR 1.200.000</div>
            <a href="learning_js1.html"><button class="btn" style="background-color: pink; width: 190px;"> <img src="./img/cart-icon.png" alt="" class="px-2"> Add to cart</button></a>
            <div class="py-3"><hr></div>
            <div><b>About Product</b></div><br>
            <div>Tailored to a level of perfection synonymous with that of a Savile Row suit and with understated quality in the detail, Jetty has been influenced by timeless 1950s style.</div> <br>
            <div>Providing a subtle nod to the past, Jetty also provides a perfect solution for the way we work today. A comprehensive product family, Jetty features a variety of elegant chairs and sofas.</div>
        </div>

    </div>
</template>
<script>
export default {
  name: 'MainPage',
  props: ["cardimage"]
}
</script>