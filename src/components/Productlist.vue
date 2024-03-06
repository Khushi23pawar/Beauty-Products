<template>
<div>
                  <h2 class="text-center py-5" >{{ title }}</h2>
               </div>
               <div class="row rightleft-padding text-center color-line" id="slider" ref="slider">
                  <div class="px-4" v-for="items,index in productObj" :key="items">

                     <div class="shop-box div1-color">
                        <div class="shop-box-inner div1-inner-color">
                           <div>
                              <img :src="items.image" alt="product" class="img-fluid"/>
                              <!-- <img src="/images/R-STCK-webtrans_540x.png" alt="product" class="img-fluid"/> -->

                            </div>
                           <div class="p-3"> {{items.image}}

                            <h3 class="text-center">{{ items.name }}</h3>
                              <p class="text-center" v-html="concatfn(index)"></p>

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

//import Image1 from '@/assets/images/R-STCK-webtrans_540x.png';
// import Image2 from '@/assets/images/image2.jpg';
// import Image3 from '@/assets/images/image3.jpg';

export default{
    name:'ProductlistCom',
    data(){
        return {
            productObj:[{
                image:"'../../public/images/R-STCK-webtrans_540x.png",
                name:"Deodarant Stick",
                details:"Rose Graninum Baking Soda Free <br> From",
                price:" $4.50 USD"


            },{
                image:"../assets/images/L-STCK-webtrans_540x.png",
                name:"Lavender Bergamot",
                details:"Lavender Bergamot <br>From ",
                price:" $4.50 USD"


            },{
                image:"../assets/images/GBSF-webtrans_388a9d91-01df-4df3-b02a-8cfca655609f_540x.png",
                name:"Grapefruit",
                details:"Grapefruit Baking Soda Free <br>From",
                price:" $4.50 USD"


            },{
                image:"../assets/images/GBSF-webtrans_388a9d91-01df-4df3-b02a-8cfca655609f_540x.png",
                name:"Grapefruit",
                details:"Grapefruit Baking Soda Free <br>From",
                price:" $4.50 USD"


            },{
                image:"../assets/images/GBSF-webtrans_388a9d91-01df-4df3-b02a-8cfca655609f_540x.png",
                name:"Grapefruit",
                details:"Grapefruit Baking Soda Free <br>From",
                price:" $4.50 USD"


            },{
                image:"../assets/images/GBSF-webtrans_388a9d91-01df-4df3-b02a-8cfca655609f_540x.png",
                name:"Grapefruit",
                details:"Grapefruit Baking Soda Free <br>From",
                price:" $4.50 USD"


            }]
        }
    },
    props:{
        title:String
    },
    mounted(){
    $(this.$refs.slider).slick({
        infinite: true,
                 loop:true,
                 slidesToShow: 3,
                 slidesToScroll:1,
                 autoplay:true,
                 dots:true,
    })
    },

    computed:{
        concatfn(){
            return function(key){
            return this.productObj[key].details+ this.productObj[key].price
            }
        }
    }
}

</script>

<style scoped>

</style>