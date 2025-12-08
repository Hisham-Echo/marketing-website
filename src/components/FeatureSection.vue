<template>
  <div class="feature-box" v-for="i in 3" :key="i">
    <div class="content">
      <div class="desc">
        <div>{{ "descripton" }}</div>
      </div>
    </div>
    <h3 class="title">{{ "Feature " }}{{ i }}</h3>
  </div>
</template>

<script>
export default {
  name: "FeatureBox",
};
</script>

<style lang="scss" scoped>
.feature-box {
  min-width: 200px;
  margin: 10px 20px;
  text-align: left;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  overflow: hidden;

  .desc {
    margin: 0;
    padding: 0;
    position: relative;
    z-index: 2;
    div {
      z-index: 3;
      position: absolute;
      top: -200px;
      width: 100%;
      height: 200px;
      padding: 10px;
      color: red;
      background-color: #00000011;
      font-size: 1rem;
      transition: top 0.3s ease-in-out;
      text-align: left;
    }
  }

  .title {
    font-size: 1.5rem;
    margin-top: 5px;
    margin-bottom: 10px;
    color: #333;
    font-weight: bold;
  }

  .content {
    font-size: 0.9rem;
    color: #555;
    background-image: url(https://placehold.co/200);
    width: 100%;
    height: 200px;
  }

  &:hover {
    .content {
      box-shadow: 0 0 10px 2px rgba(0, 0, 0, 0.2);
      // transform: scale(1.1);
    }
    .desc div {
      top: 0;
    }
  }
}
</style>
