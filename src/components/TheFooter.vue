<script>
export default {
   name: "TheFooter",
   data() {
      return {
         footerLinks: [
            {
               title: "DC COMICS",
               links: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"]
            },
            {
               title: "SHOP",
               links: ["Shop DC", "Shop DC Collectables"]
            },
            {
               title: "DC",
               links: ["Terms Of Use", "Provacy Policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contast Us"]
            },
            {
               title: "SITES",
               links: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"]
            },
         ]
      };
   },
   methods: {
      stampiamo(test) {
         console.log(test);
      }
   }
}
</script>

<template>
   <div class="sfondo">
      <div class="container py-5 d-flex justify-content-between">
         <div class="liste">
            <ul v-for="(gruppo, i) in footerLinks">
               <h3>{{ gruppo.title }}</h3>
               <li>{{ gruppo.links }}</li>
            </ul>
         </div>
         <img src="../../public/img/dc-logo-bg.png" alt="">
      </div>
   </div>
</template>

<style scoped>
   .sfondo{
      /* background-image: url(../../public/img/footer-bg.jpg); */
      background-repeat: no-repeat;
      background-size: cover;
      
   }
</style>

