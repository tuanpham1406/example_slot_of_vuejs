<template>
  <div>
    <h1>This is Contact page</h1>
    <button class="btn btn-outline-primary" @click="counter++">Increment Value</button>
    <p>{{counter}}</p>
  </div>
</template>

<script>
    export default {
        name: "Contact",
        data: () => ({
            counter: 0
        }),
        created() {
          console.log("Created!")
        },
        destroyed() {
            console.log('Destroyed!')
        },
        deactivated() {
            console.log("Deactivated!")
        },
        activated() {
            console.log("Activated!")
        }
    }
</script>

<style scoped>

</style>
