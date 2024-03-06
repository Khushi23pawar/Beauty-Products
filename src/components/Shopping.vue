<template>
  <div class="pt-5">
               <div class="row">
                  <div class="col-md-6 packaging-img-box">
                  </div>
                  <div class="col-md-6">
                     <div>
                        <h3 class="text-center p-4">{{ tittle }}</h3>
                         <div id="slider3" ref="slider">
                           <div class="col-12" v-for="items,index in shoppingObj" :key="items">

                              <div class=" slider3-image">
                                 <img src="../assets/images/RE-LIP-webtrans_360x.png" alt="product" class="img-fluid"/>
                              </div>
                              <div class=" text-center    p-3">
                                 <h3 >{{ items.name }}</h3>
                                 <p v-html="concatfn(index)" ></p>
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
    },
    props:{
      tittle: String
    },
    data(){
      return{
         shoppingObj:[{
                image:"../assets/images/RE-LIP-webtrans_360x.png",
                name:"Deodarant Stick",
                details:"Rose Graninum Baking Soda Free <br> From",
                price:" $4.50 USD"
         },{
                image:"../assets/images/JC-FO_360x.png",
                name:"Deodarant Stick",
                details:"Lavender Bergamot <br>From",
                price:" $4.50 USD"
         },{
                image:"../assets/images/LG-BO-webtrans_360x.png",
                name:"Deodarant Stick",
                details:"Grapefruit Baking Soda Free <br>From",
                price:" $4.50 USD"
         },{
                image:"../assets/images/RC-FO-webtrans_540x.png",
                name:"Deodarant Stick",
                details:"Rose Graninum Baking Soda Free <br> From",
                price:" $4.50 USD"
         },
      
      
      
      
      ]
      }
    },
    computed:{
        concatfn(){
            return function(key){
            return this.shoppingObj[key].details+ this.shoppingObj[key].price
            }
        }
    }
}
</script>

<style scoped>
.packaging-img-box{
    background-image: url("../assets/images/meow-meow-tweet-new-packaging_900x.jpg" );
}
</style>