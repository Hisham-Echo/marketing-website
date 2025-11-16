<template>
  <div class="home">
    <div class="banner img-wrapper container-fluid p-0 position-relative">
      <div class="overlay z-3 position-absolute p-5">
        <h1>HEADPHONES</h1>
      </div>
      <img
        src="../assets/imgs/silivan-munguarakarama-NrR9gn3lFKU-unsplash.jpg"
        alt="banner"
      />
    </div>

    <div class="desc container-sm">
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores ipsam
      </p>
      <p>
        Debitis aperiam iure laborum mollitia porro quisquam ipsam illum, eaque
      </p>
      <p>
        Quisquam ipsam illum, eaque debitis aperiam iure laborum mollitia porro.
      </p>
    </div>

    <div
      class="feat container-fluid d-flex justify-content-center align-items-center flex-wrap"
    >
      <feature-box />
      <feature-box />
      <feature-box />
    </div>

    <div class="footer bg-danger text-center container-sm">
      <p>footer</p>
      <button>Contact Us</button>
    </div>
  </div>
</template>

<script>
import FeatureBox from "@/components/FeatureBox.vue";
export default {
  components: { FeatureBox },
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
    background: #00000025;
    border-radius: 10px;
    padding: 20px;
  }
}

img {
  width: 100%;
  height: 40vh;
  object-fit: cover;
}

.desc {
  margin: 20px auto;
  padding: 10px;
  text-align: center;
}

.desc p {
  margin: 0;
  padding: 5px;
  margin: 10px 0;
  font-size: 1.2rem;
  background: #ff008015;
  border: 2px solid #ff008005;
  border-radius: 5px;
  &:hover {
    background: #ff008020;
  }
}
.feat {
  // height: 200px;
  padding: 40px 20px;
  margin: 20px 0;
}
</style>
