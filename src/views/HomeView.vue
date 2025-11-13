<template>
  <div class="home bg-primary">
    <div class="banner img-wrapper conatiner-fluid">
      <div class="overlay z-3 position-absolute p-5">
        <h1>HEADPHONES</h1>
      </div>
      <img
        src="../assets/imgs/silivan-munguarakarama-NrR9gn3lFKU-unsplash.jpg"
        alt="banner"
      />
    </div>

    <div class="desc container-sm bg-danger">description</div>

    <div class="feat container-fluid bg-warning">feats components</div>

    <div class="footer bg-danger text-center container-sm">
      <p>footer</p>
      <button>Contact Us</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeView",
};
</script>

<style lang="scss">
.img-wrapper {
  width: 100%;
  height: 40vh;
  overflow: hidden;
  position: relative;
}

.overlay {
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.4);
  color: white;
  h1 {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 4rem;
  }
}

img {
  width: 100%;
  height: 40vh;
  object-fit: cover;
}
</style>
