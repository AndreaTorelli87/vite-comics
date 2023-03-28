<script>
   export default {
      name: "MyCard",
      props: {
         image: String,
         price: String,
         title: String,
         type: String
      }
   }
</script>

<template>

   <div class="card">
      <img :src="image" :alt="title"/>
      <h6 class="py-2 text-white">{{ title }}</h6>
   </div>

</template>

<style scoped> 
   .card{
      width: calc(100% / 6 );
      background-color: transparent;
   }

   img{
      object-fit: cover;
      height: 12rem;
      object-position: top;
   }

</style>