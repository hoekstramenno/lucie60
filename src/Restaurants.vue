<template>
  <div>
    <div class="container restaurants">
      <h1 class="title">Kies een restaurant</h1>
      <card
        data-image="https://lh3.googleusercontent.com/proxy/UUCaC1atYOfrMAPQYQB3D7OfESTZIgYkeQzkPHfI1w7hgkAL0Ze5qO3BLORcE9rfEXpdsKv3VGAX7zqLO38jOzIELw">
        <h1 slot="header">Tent</h1>
        <p slot="content">Houtskool restaurant</p>
      </card>
      <card
        data-image="https://d1ralsognjng37.cloudfront.net/5b8f7e20-3ee1-481b-8b73-1e8421a4d48f.jpeg">
        <h1 slot="header">Nagoya</h1>
        <p slot="content">Sushi</p>
      </card>
      <card
        data-image="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTArHTeiIyKu9eJOUqdGrM84FGjmOfsTqS8Rw&usqp=CAU">
        <h1 slot="header">La Cubanita</h1>
        <p slot="content">Tapas</p>
      </card>
      <card
        data-image="https://www.francescakookt.nl/wp-content/uploads/2016/10/restauranttips_3_zarzo_bakkerswinkel_table24_uitgelicht_1.jpg">
        <h1 slot="header">Table 24</h1>
        <p slot="content">Kleine hapjes en/of hoofdgerechten</p>
      </card>
      <card
        data-image="https://media-cdn.tripadvisor.com/media/photo-s/18/da/8a/2a/gerecht-bij-the-louisiana.jpg">
        <h1 slot="header">Lousiana</h1>
        <p slot="content">Amerikaans</p>
      </card>
      <card
        data-image="https://i.pinimg.com/originals/a4/ba/77/a4ba77c66119a103ca672cd8a78856fc.jpg">
        <h1 slot="header">Villa westend</h1>
        <p slot="content">Lekker aan een meertje</p>
      </card>
      <card
        data-image="https://upload.wikimedia.org/wikipedia/commons/thumb/6/67/Fries_2.jpg/2560px-Fries_2.jpg">
        <h1 slot="header">Snackbar het Plein</h1>
        <p slot="content">Patat della mayonaise.</p>
      </card>
      <card
        data-image="https://www.anne-wies.nl/wp-content/uploads/2019/12/Welke-wijn-bij-kaviaar-uitgelicht.jpg">
        <h1 slot="header">... of iets anders</h1>
        <p slot="content">Genoeg te eten</p>
      </card>
    </div>
  </div>
</template>

<script>
  import Card from './Card.vue'

  export default {
    name      : 'Restaurants',
    components: {
      Card
    },
  }

</script>

<style lang="scss">

  .title {
    font-family: "Raleway";
    font-size: 24px;
    font-weight: 700;
    color: #5D4037;
    text-align: center;
    width: 100%;
  }

  .restaurants {
    margin: 30px 0;
  }

  .card-wrap {
    margin: 10px;
    transform: perspective(800px);
    transform-style: preserve-3d;
    cursor: pointer;
    // background-color: #fff;
  }

</style>
