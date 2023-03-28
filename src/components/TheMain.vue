<script>
import MyCard from './MyCard.vue';
export default {
   components: {
      MyCard
   },
   data() {
      return {
         comics: [
            {
               "thumb": "https://static.dc.com/2023-03/LEGIONOB_Cv1_00111_DIGITAL.jpg?w=640",
               "price": "$19.99",
               "series": "Action Comics",
               "type": "comic book"
            },
            {
               "thumb": "https://static.dc.com/2023-03/BA_Cv9_00911_DIGITAL.jpg?w=640",
               "price": "$3.99",
               "series": "American Vampire 1976",
               "type": "comic book"
            },
            {
               "thumb": "https://static.dc.com/2023-03/ST_GH_Cv3_00311_DIGITAL.jpg?w=640",
               "price": "$16.99",
               "series": "Aquaman",
               "type": "graphic novel"
            },
            {
               "thumb": "https://static.dc.com/2023-03/MS30A_Cv1_00111_DIGITAL.jpg?w=640",
               "price": "$2.99",
               "series": "Batgirl",
               "type": "comic book"
            },
            {
               "thumb": "https://static.dc.com/2023-03/MS30A_Cv1_00111_DIGITAL.jpg?w=640",
               "price": "$3.99",
               "series": "Batman",
               "type": "comic book"
            },
            {
               "thumb": "https://static.dc.com/2023-03/BMSMWF_Cv13_01311_DIGITAL.jpg?w=640",
               "price": "$2.99",
               "series": "Batman Beyond",
               "type": "comic book"
            },
            {
               "thumb": "https://static.dc.com/2023-03/NTW_Cv102_10211_DIGITAL-1.jpg?w=640",
               "price": "$3.99",
               "series": "Batman/Superman",
               "type": "comic book"
            },
            {
               "thumb": "https://static.dc.com/2023-03/FLS_Cv795_79511_DIGITAL.jpg?w=640",
               "price": "$4.99",
               "series": "Batman/Superman Annual",
               "type": "comic book"
            },
            {
               "thumb": "https://static.dc.com/2023-03/DCConnect_35-CVR.jpg?w=640",
               "price": "$5.99",
               "series": "Batman: The Joker War Zone",
               "type": "comic book"
            },
            {
               "thumb": "https://static.dc.com/2023-03/ROBIN_v3%20%28Cover%29.jpg?w=640",
               "price": "$6.99",
               "series": "Batman: Three Jokers",
               "type": "comic book"
            },
            {
               "thumb": "https://static.dc.com/2023-03/LP-ROTG_Cv1_00111_DIGITAL.jpg?w=640",
               "price": "$4.99",
               "series": "Batman: White Knight Presents: Harley Quinn",
               "type": "comic book"
            },
            {
               "thumb": "https://static.dc.com/2023-03/SM_LOST_Cv1_00111_DIGITAL.jpg?w=640",
               "price": "$16.99",
               "series": "Catwoman",
               "type": "graphic novel"
            }
         ]
      }
   }
}   
</script>

<template>
   <div id="jumbo"></div>
   <div class="sfondo">
      <div class="container">
         <h2 class="text-white fw-bold p-3 d-inline-block">CURRENT SERIES</h2>
      </div>
      <div class="container pt-5 d-flex flex-wrap">
         <div class="row">
            <MyCard v-for="comic in comics"
         :image="comic.thumb"
         :price="comic.price"
         :title="comic.series"
         :type="comic.type"
         />
         </div>
      </div>
   </div>
</template>

<style scoped>

#jumbo{
   background-image: url(../../public/img/jumbotron.jpg);
   height: 43vh;
}
.sfondo {
   background-color: black;
}

h2{
   background-color: #0282F9;
   margin: -2rem 0;
}
</style>