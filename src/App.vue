<template>
  <div id="app">
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <app-card cartWords="Meow">
            <h2 slot="title">{{cardTitle}}</h2>
            <p>white Cat is so noob!</p>
          </app-card>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
    import Card from "./components/Card.vue";

    export default {
        components: {
            appCard: Card
        },
        data: () => ({
            cardTitle: 'White Cat'
        })
    };
</script>

<style>
</style>
