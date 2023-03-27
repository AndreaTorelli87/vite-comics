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
         <button>SIGN-UP NOW!</button>
         <div>
            <span>FOLLOW US</span>
            <img v-for="icon in socialIcons" :src="'../../public/img/footer-' + icon +'.png'" :alt="'Logo' + icon" class="px-2">
         </div>
      </div>
   </div>
</template>

<style scoped>

   .sfondo{
      background-color: #303030;
      height: 11vh;
   }

</style>