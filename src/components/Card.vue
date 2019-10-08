<template>
  <div>
    <div class="title">
      <slot name="title"></slot>
      <span>
<!--        slot have value default which is slot default-->
        <slot name="subTitles">The SubTitles</slot>
      </span>
    </div>
    <div class="content">
      <!--slot unsign is default slot-->
      <slot></slot>
    </div>
  </div>
</template>

<script>
    export default {
        props: ["cartWords"]
    };
</script>

<style scoped>
  div {
    widows: 100;
    border: 1px solid #ccc;
    box-shadow: 1px 1px 2px rgba(0, 0, 0, 0.6);
    padding: 30px;
    margin: 20px auto;
    text-align: center;
  }

  h2 {
    color: red;
  }
</style>
