<template>

   <div class="main-con">
    <!-- start header -->
    <HeaderCom/>
        <!-- end header -->

    <!-- start landingpage -->

         <div class="main-con-inner">
            <div class="landing-con">
               <div class="landing-inner-con text-center" >
                  <h2 v-html="landingHeading" ></h2>
                  <p v-html="landingPara"></p>
                  <button type="btn" class="btn">READ MORE</button>
               </div>

            </div>
                <!-- end landingpage -->
    <!-- start marcquee line -->

            <MarcqueeCom/>
                <!-- end marcquee line -->
    <!-- start productlist  -->

            <ProductlistCom title="shopping Our Bestsellers"/>
                <!-- end productlist  -->

            <!-- start video  -->
            <div class="video-box rightleft-padding text-center">
               <video src="./assets/images/cosmetic-video.mp4"  muted class="object-fit" autoplay></video>
            </div>
            <!-- end video -->
            <!-- start skin type  -->
            <ProductlistCom title="shop by my skin type"/>
<!-- end skin type -->
<!-- start about us -->
<div class="about-us-main-con rightleft-padding">
               <div class="about-us-con">
                  <div class="text-center about-us-inner-con">
                     <h3>WE ARE</h3>
                     <p>Vegan personal care for every body. Always<br> ethical, low-waste, handmade & cruelty-free.</p>
                     <button type="btn" class="btn">ABOUT US</button>
                  </div>
               </div>
            </div>
            <!-- end about us -->
            <!-- start shopping  -->
            <ShoppingCom tittle="Shop Our New Packaging"/>
<!-- end shopping -->
<!-- start readlatest -->
<ReadlatestCom title="Read the Latest"/>


<!-- end readlatest -->
<!-- start 2 marquee -->
<MarcqueeCom/>

<!-- end 2 marquee -->
<!-- start footer -->
<FooterCom/>
<!-- end footer -->
            </div>

            </div>
          


</template>

<script>
 import HeaderCom from './components/Header.vue'
 import MarcqueeCom from './components/Marcquee.vue'
 import ProductlistCom from './components/Productlist.vue'
 import ShoppingCom from './components/Shopping.vue'
 import ReadlatestCom from './components/Readlatest.vue'
 import FooterCom from './components/Footer.vue'




export default {
  name: 'App',
  components: {
     HeaderCom,
     MarcqueeCom,
     ProductlistCom,
     ShoppingCom,
     ReadlatestCom,
     FooterCom
  },
  data(){
    return{
      landingHeading:"On Finding Comfort<br> In Your Own Skin",
      landingPara:"What if moisturizing our bodies has been <br>about comfort this whole time?",
      //videoUrl:'./assets/images/cosmetic-video.mp4'
    
    
    }
  }
}
</script>

<style scoped>



.landing-con{
    width: 100%;
    height: 95vh;
    position: relative;
    background-image: url("./assets/images/banner-body-oil-nails_1512x.png");
}

.about-us-con{
    background-image: url("./assets/images/ARTWORK_KITS_MIG_0b18e60e-93f1-42a8-b7f1-4d08f833ccba.png");
   
}

    



</style>
