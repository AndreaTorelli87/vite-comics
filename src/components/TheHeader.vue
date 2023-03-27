<script>
export default {
  name: "TheHeader",
  data() {
    return {
      navLinks: ["CHARACTERS", "COMICS", "MOVIES", "TV", "GAMES", "COLLECTIBLES", "VIDEOS", "FANS", "NEWS", "SHOP"],
      message: "sono l'header"
    };
  },
};
</script>

<template>
   <div class="container d-flex justify-content-between p-3">
      <img src="../../public/img/dc-logo.png" alt="Logo DC">
      <ul class="d-flex justify-content-center align-items-center list-unstyled">
         <li v-for="link in navLinks" class="p-3"><a :href="link" class="text-decoration-none text-black fw-bold">{{ link }}</a></li>
      </ul>
   </div>
</template>

<style>


</style>