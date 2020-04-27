<template>
  <div class="nav-bar">
    <div class="left">
      <slot name="letf"></slot>
    </div>
    <div class="center">
      <slot name="center"></slot>
    </div>
    <div class="right">
      <slot name="right"></slot>
    </div>
  </div>
</template>

<script>
  export default {
    name: "NavBar"
  }
</script>

<style scoped>
  .nav-bar{
    display: flex;
    height: 44px;

    /*color: #f6f6f6;*/
    text-align: center;
    line-height: 44px;
    /*background-color: #ff4200;*/
    box-shadow: 0 1px 1px rgba(100,100,100,0.1);
  }
  .left, .right{
    width: 60px;
  }
  .center{
    flex: 1;
  }

</style>
