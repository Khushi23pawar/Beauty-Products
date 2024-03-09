<template>
   <!-- start read the latest section -->
   <div class="pt-5">
                <h2 class="text-center p-4">{{ title }}</h2>
                <div class="row rightleft-padding">
                    <div class="col-md-3" v-for="items,index in readObj" :key="items">
                            <div class="read-bg-color" :class="{'circle-box':index % 2 !==0}">
                            <div class="read-image-con" :class="{'circle-inner-box':index % 2 !==0}">
                                <img src="../assets/images/meow-meow-tweet-holiday-aromatherapy_540x.jpg" alt="product" class="img-fluid"/>
                            </div>
                            </div>
                            <div class="read-contain">
                                <h4 class="pt-3">{{ items.headline }}</h4>
                                <p>{{ items.description }}</p>
                                <button>Read More</button>
                            </div>
                    </div>
                  
                 
          </div>
            </div>
    <!-- end read the latest section -->
</template>
<script>
export default{
    name:'ReadlatestCom',
    data(){
        return{
            readObj:[{
                image:"",
                headline:"Earth & Air Aromatherapy Bundles",
                description:"Two new aromatherapeutic  product lines for grounding & uplifting",
                link:"",

            },
            { image:"",
                headline:"A Guide to Slow Living for November",
                description:"How to snail-crawl your way through the month, one anti-consumerist activity at a time.",
                link:"",
            },
            { image:"",
                headline:"Earth & Air Aromatherapy Bundles",
                description:"Two new aromatherapeutic  product lines for grounding & uplifting",
                link:"",
            },
            { image:"",
                headline:"A Guide to Slow Living for November",
                description:"How to snail-crawl your way through the month, one anti-consumerist activity at a time.",
                link:"",
            },
            ]

        }
    },
    props:{
        title:String
    },
}

</script>
<style scoped>
</style>