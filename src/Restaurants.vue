<template>
  <div>
    <div class="container restaurants">
      <h2 class="title">Kies een restaurant</h2>
      <card
        data-image="https://lh3.googleusercontent.com/proxy/7im7sjtPtHGk8jRVIcFjVdkASe0M5bEnLyGbT8HLb37E-kVGE8XWy5wAdNP19vNJG7L0xlkSHlRTHqUqjTWhCp886Wo1mdjbfq3MMJ3GpjDOow">
        <h2 slot="header">Tent</h2>
        <p slot="content">Houtskool restaurant</p>
      </card>
      <card
        data-image="https://d1ralsognjng37.cloudfront.net/5b8f7e20-3ee1-481b-8b73-1e8421a4d48f.jpeg">
        <h2 slot="header">Nagoya</h2>
        <p slot="content">Sushi</p>
      </card>
      <card
        data-image="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTArHTeiIyKu9eJOUqdGrM84FGjmOfsTqS8Rw&usqp=CAU">
        <h2 slot="header">La Cubanita</h2>
        <p slot="content">Tapas</p>
      </card>
      <card
        data-image="https://www.francescakookt.nl/wp-content/uploads/2016/10/restauranttips_3_zarzo_bakkerswinkel_table24_uitgelicht_1.jpg">
        <h2 slot="header">Table 24</h2>
        <p slot="content">Kleine hapjes en/of hoofdgerechten</p>
      </card>
      <card
        data-image="https://media-cdn.tripadvisor.com/media/photo-s/18/da/8a/2a/gerecht-bij-the-louisiana.jpg">
        <h2 slot="header">Lousiana Haarlem</h2>
        <p slot="content">Amerikaans diner</p>
      </card>
      <card
        data-image="https://i.pinimg.com/originals/a4/ba/77/a4ba77c66119a103ca672cd8a78856fc.jpg">
        <h2 slot="header">Villa westend</h2>
        <p slot="content">Lekker aan een meertje</p>
      </card>
      <card
        data-image="https://upload.wikimedia.org/wikipedia/commons/thumb/6/67/Fries_2.jpg/2560px-Fries_2.jpg">
        <h2 slot="header">Snackbar het Plein</h2>
        <p slot="content">Patat della mayonaise.</p>
      </card>
      <card
        data-image="https://www.anne-wies.nl/wp-content/uploads/2019/12/Welke-wijn-bij-kaviaar-uitgelicht.jpg">
        <h2 slot="header">... of iets anders</h2>
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
