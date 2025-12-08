<template>
  <nav
    class="p-3 container-fluid d-flex align-items-center justify-content-between"
  >
    <router-link to="/">
      <img src="@/assets/logo.png" alt="logo" />
    </router-link>
    <div>
      <router-link to="/explore">Explore</router-link>
      <router-link to="/about">About</router-link>
      <router-link to="/support">Support</router-link>
    </div>
  </nav>
</template>
<style>
nav {
  position: absolute;
  top: 0;
  z-index: 1000;
  background-color: #0000002f;
  padding: 30px;
  a {
    font-weight: bold;
    color: #ffffffaa;
    margin: 0 10px;
    text-decoration: none;
    img {
      height: 50px;
    }
    &:hover {
      color: #ffffffff;
    }

    &.router-link-exact-active {
      color: #ffffffaa;
      border-color: #000000;
    }
  }
}
</style>
<script>
export default {
  name: "NavBar",
};
</script>
