<template>
  <div class="home-container">
    <el-carousel class="home-carousel">
      <el-carousel-item v-for="item in arr" :key="item.name">
        <h3>{{ item.name }}</h3>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<script>
export default {
  data() {
    return {
      arr: [{ name: 'one' }, { name: 'two' }, { name: 'three' }]
    };
  }
};
</script>

<style scoped lang="scss" rel="stylesheet/scss">
@import '../../assets/scss/variables';
@import '../../assets/scss/mixins';
.home-container {
  .home-carousel {
    width: 100%;
    height: 300px;
    background-color: aquamarine;
  }
}
</style>