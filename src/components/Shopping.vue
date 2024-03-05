<template>
  <div class="pt-5">
               <div class="row">
                  <div class="col-md-6 packaging-img-box">
                  </div>
                  <div class="col-md-6">
                     <div>
                        <h3 class="text-center p-4">Shop Our New Packaging</h3>
                        <div id="slider3" ref="slider">
                           <div class="col-12">
                              <div class=" slider3-image">
                                 <img src="../assets/images/RE-LIP-webtrans_360x.png" alt="product" class="img-fluid"/>
                              </div>
                              <div class=" text-center    p-3">
                                 <h3 >Deodarant Stick</h3>
                                 <p >Grapefruit Baking Soda Free <br>From $4.50 USD</p>
                              </div>
                           </div>
                            <div class="col-12">
                              <div class="slider3-image">
                                 <img src="../assets/images/JC-FO_360x.png" alt="product" class="img-fluid"/>
                              </div>
                              <div class="p-3 text-center">
                                 <h3>Deodarant Stick</h3>
                                 <p >Lavender Bergamot <br>From $4.50 USD</p>
                              </div>
                           </div>
                           <div class="col-12">
                              <div class=" slider3-image">
                                 <img src="../assets/images/LG-BO-webtrans_360x.png" alt="product" class="img-fluid"/>
                              </div>
                              <div class=" text-center    p-3">
                                 <h3 >Deodarant Stick</h3>
                                 <p >Grapefruit Baking Soda Free <br>From $4.50 USD</p>
                              </div>
                           </div>
                           <div class="col-12">
                              <div class=" slider3-image">
                                 <img src="../assets/images/RC-FO-webtrans_540x.png" alt="product" class="img-fluid"/>
                              </div>
                              <div class=" text-center    p-3">
                                 <h3 >Deodarant Stick</h3>
                                 <p >Grapefruit Baking Soda Free <br>From $4.50 USD</p>
                              </div>
                           </div> 
                        </div>
                     </div>
                  </div>
               </div>
            </div>
</template>


<script>
import $ from 'jquery';
import 'slick-carousel/slick/slick.css';
import 'slick-carousel/slick/slick';
export default{
    name:'ShoppingCom',
    mounted(){
    $(this.$refs.slider).slick({
        infinite: true,
                 slidesToShow: 1,
                 slidesToScroll:1,
                 autoplay:true,
                 dots:true,
    })
    }
}
</script>

<style scoped>
.packaging-img-box{
    background-image: url("../assets/images/meow-meow-tweet-new-packaging_900x.jpg" );
}
</style>