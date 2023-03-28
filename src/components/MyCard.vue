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
      <div class="imgWrapper">
         <img :src="image" :alt="title" />
      </div>
      <h6 class="my-2 text-white">{{ title }}</h6>
   </div>
</template>

<style lang="scss" scoped> 
.card {
   width: calc(100% / 6);
   background-color: transparent;
}

.imgWrapper{
   overflow: hidden;
}

img {
   height: 15rem;
   transition: scale 1s;

   &:hover{
      scale: 1.1;
   }
}
</style>