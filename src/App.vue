<template>
  <nav
    class="bg-primary-subtle p-3 container-fluid d-flex align-items-center justify-content-between"
  >
    <router-link to="/">
      <img src="./assets/logo.png" alt="logo" />
    </router-link>
    <div>
      <router-link to="/explore">Explore</router-link>
      <router-link to="/about">About</router-link>
      <router-link to="/support">Support</router-link>
    </div>
  </nav>
  <router-view />
</template>

<style lang="scss">
* {
  transition: 0.2s ease-in-out all;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #00000095;
    margin: 0 10px;
    text-decoration: none;
    img {
      height: 50px;
    }
    &:hover {
      color: #000000;
    }

    &.router-link-exact-active {
      color: #000000;
      border-color: #000000;
    }
  }
}
</style>
