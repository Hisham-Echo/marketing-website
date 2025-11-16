<template>
  <div class="feature-box">
    <h3 class="title">{{ "title" }}</h3>
    <p class="description">{{ "description" }}</p>
    <div class="content">
      <slot>content</slot>
    </div>
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
  background: #3697ffc5;
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 20px;
  margin: 10px 20px;
  text-align: center;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);

  &:hover {
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
    transform: scale(1.1);
  }

  .title {
    font-size: 1.5rem;
    margin-bottom: 10px;
    color: #333;
  }

  .description {
    font-size: 1rem;
    margin-bottom: 15px;
    color: #666;
  }

  .content {
    font-size: 0.9rem;
    color: #555;
  }
}
</style>
