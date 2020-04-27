<template>
  <div class="recommend">
    <div v-for="item in recommends" class="recommend-item">
      <a :href="item.link">
        <img :src="item.image" alt="">
        <div>{{item.title}}</div>
      </a>
    </div>
  </div>
</template>

<script>
  export default {
    name: "RecommendVeiw",
    props:{
      recommends:{
        type: Array,
        default() {
          return [];
        }
      }
    }
  }
</script>

<style scoped>
  .recommend{
    display: flex;
    text-align: center;
    font-size: 12px;

    padding: 10px 0 15px;
    border-bottom: 10px solid #f2f2f2;
  }

  .recommend-item{
    flex: 1;
  }

  .recommend-item img{
    width: 68px;
    height: 68px;
    margin-bottom: 10px;
  }
</style>
