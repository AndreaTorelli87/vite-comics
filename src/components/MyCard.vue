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

   <div class="p-2">
      <img :src="image" :alt="title"/>
      <h5>{{ title }}</h5>
      <h3 class="text-white">prova</h3>
   </div>

</template>

<style>

</style>