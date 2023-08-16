<template>
  <div class="main">
    <img alt="DTT logo" src="../assets/images/dtt_logo_black.svg" class="hideInMobile" />

    <router-link to="/">
      <p class="hideInMobile">Houses</p>
      <span class="material-symbols-outlined showInMobile"> home </span>
    </router-link>

    <router-link to="/about">
      <p class="hideInMobile">About</p>

      <span class="material-symbols-outlined showInMobile"> info </span>
    </router-link>
  </div>
</template>

<script setup>
</script>

<style scoped>
.main {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  font-size: 1.2em;
  padding: 0% 15%;
  background-color: white;
  height: 13vh;
}

img {
  height: 7em;
  width: 7em;
}

nav {
  padding: 20px;
}

nav a {
  color: #1e1519;
  margin: 0% 5%;
  text-decoration: none;
}

nav a.router-link-exact-active {
  font-weight: bolder;
}
.showInMobile {
  display: none;
}
.hideInMobile {
  display: block;
}
@media only screen and (max-width: 768px) {
  .showInMobile {
    display: block;
  }
  .hideInMobile {
    display: none;
  }
  .main {
    justify-content: space-around;
  }
}
</style>
