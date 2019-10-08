<template>
  <div id="app">
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <button class="btn btn-outline-danger" @click="selectComponent= 'appCard'">Card</button>
          <button class="btn btn-outline-danger" @click="selectComponent= 'appAbout'">About</button>
          <button class="btn btn-outline-danger" @click="selectComponent= 'appContact'">Contact</button>
        </div>
      </div>
      <div class="row">
        <div class="col-sm-12">
          <!--          <div><p>{{selectComponent}}</p></div>-->
          <!--          <app-card cartWords="Meow">-->
          <!--            <h2 slot="title">{{cardTitle}}</h2>-->
          <!--            <p>white Cat is so noob!</p>-->
          <!--          </app-card>-->
          <keep-alive>
            <component :is="selectComponent"></component>
          </keep-alive>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
    import Card from "./components/Card.vue";
    import Contact from "./components/Contact";
    import About from "./components/About";

    export default {
        components: {
            appCard: Card,
            appContact: Contact,
            appAbout: About,
        },
        data: () => ({
            cardTitle: 'White Cat',
            selectComponent: 'appCard'
        })
    };
</script>

<style>
</style>
