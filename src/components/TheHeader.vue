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
    <img src="../../public/img/dc-logo.png" alt="Logo DC" class="p-3">
    <ul class="d-flex list-unstyled m-0">
      <li v-for="link in navLinks" class="px-3">
        <a :href="link" class="text-decoration-none fw-bold">{{ link }}</a>
      </li>
    </ul>
  </div>
</template>

<style lang="scss" scoped>
li {
  padding: 50px 0;
  border-bottom: solid 6px white;

  &:hover {
    border-bottom: solid 6px #0282F9;

    a {
      color: #0282F9;
    }
  }
}

a {
  color: black;
}
</style>