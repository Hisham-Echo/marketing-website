<template>
  <div class="home">
    <!-- landing banner and title -->
    <div class="banner img-wrapper container-fluid p-0 position-relative">
      <div class="overlay z-3 position-absolute p-5">
        <h1>HEADPHONES</h1>
      </div>
      <img
        src="../assets/imgs/silivan-munguarakarama-NrR9gn3lFKU-unsplash.jpg"
        alt="banner"
      />
    </div>
    <!-- descripotion section -->
    <div
      class="desc container-sm d-flex flex-column justify-content-center align-items-center"
    >
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
    <!-- feature section -->
    <div
      class="feat container-fluid d-flex justify-content-center align-items-center flex-wrap"
    >
      <feature-box />
    </div>
    <!-- footer section -->
    <footer class="text-center container-sm">
      <p>
        mollitia eos id ipsum Minima nulla impedit rerum derum dignissimos hic!
      </p>
      <button>Contact Us</button>
    </footer>
  </div>
</template>

<script>
import FeatureBox from "@/components/FeatureSection.vue";
export default {
  components: { FeatureBox },
  name: "HomeView",
};
</script>

<style lang="scss">
.img-wrapper {
  width: 100%;
  height: 60vh;
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
  height: 60vh;
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
  text-align: center;
  width: 60%;
  @media (max-width: 787px) {
    width: 100%;
  }
  max-width: 700px;
  &:hover {
    background: #ff008020;
  }
}
.feat {
  padding: 40px 20px;
  margin: 20px 0;
}

footer {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 40px auto;
  p {
    font-size: 1.2rem;
    background-color: #ff008015;
    padding: 5px 20px;
    width: 70%;
    @media (max-width: 787px) {
      width: 100%;
    }
  }
  button {
    color: white;
    border: none;
    font-size: 2rem;
    font-weight: bold;
    padding: 5px 40px;
    background-color: #0d6efd;
    &:hover {
      background-color: #0d6efdcc;
    }
  }
}
</style>
