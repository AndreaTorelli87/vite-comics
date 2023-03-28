<script>
export default {
   name: "BlueBar",
   data() {
      return {
         shop: [
            {
               image: "public/img/buy-comics-digital-comics.png",
               text: "DIGITAL COMICS"
            },{
               image: "public/img/buy-comics-merchandise.png",
               text: "DC MERCHANDISE"
            },{
               image: "public/img/buy-comics-subscriptions.png",
               text: "SUBSCRIPTION"
            },{
               image: "public/img/buy-comics-shop-locator.png",
               text: "COMIC SHOP LOCATOR"
            },{
               image: "public/img/buy-dc-power-visa.svg",
               text: "DC POWER VISA"
            },
         ],
      };
   },
};

</script>


<template>
   <div class="sfondo">
      <div class="container h-100">
         <div class="row h-100">
            <div v-for="article in shop" class="col d-flex align-items-center">
               <img :src="article.image" :alt="article.text">
               <span class="text-white">{{ article.text }}</span>
            </div>
         </div>
      </div>
   </div>
</template>


<style lang="scss" scoped>
   .sfondo{
      background-color: #0282F9;
      height: 10rem;
   }

   img{
      height: 3rem;
      padding-right: 1rem;
   }

   span{
      font-size: 14px;
   }
</style>