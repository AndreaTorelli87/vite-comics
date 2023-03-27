<script>
export default {
   name: "Cta",
   data() {
    return {
      socialIcons: ["facebook", "periscope", "pinterest", "twitter", "youtube"],
    };
  },
}
</script>

<template>
   <div class="sfondo">
      <div class="container d-flex justify-content-between align-items-center">
         <button class="text-white fw-bold p-2">SIGN-UP NOW!</button>
         <div>
            <span class="fw-bold px-2">FOLLOW US</span>
            <a v-for="icon in socialIcons" href="#">
               <img :src="'../../public/img/footer-' + icon +'.png'" :alt="'logo ' + icon" class="px-2">
            </a>
         </div>
      </div>
   </div>
</template>

<style scoped>

   .sfondo{
      background-color: #303030;
   }

   .container{
      height: 15vh;
   }

   span{
      color: #0282F9;
   }

   button{
      border: solid 2px #0282F9;
      background-color: transparent;
   }

</style>