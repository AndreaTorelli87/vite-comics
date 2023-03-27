<script>
export default {
  name: "TheHeader",
  data() {
    return {
      navLinks: ["CHARACTERS", "COMICS", "MOVIES", "TV", "GAMES", "COLLECTIBLES", "VIDEOS", "FANS", "NEWS", "SHOP"],
    };
  },
};
</script>

<template>
  <div class="container d-flex justify-content-between">
    <img src="../../public/img/dc-logo.png" alt="Logo DC">
    <ul class="d-flex justify-content-center align-items-center list-unstyled h-100 m-0">
      <li v-for="link in navLinks" class="px-3">
        <a :href="link" class="text-decoration-none text-black fw-bold">{{ link }}</a>
      </li>
    </ul>
  </div>
</template>

<style scoped>
  li{
    padding: 31px 0;
  }

  li:hover{
    border-bottom: solid 6px #0282F9;
    padding: 37px;
  }

  li:hover a{
    color: #0282F9;
  }
</style>