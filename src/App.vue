<template>
  <div id="app">
    <b-navbar type="dark" variant="dark">
      <b-navbar-nav>
        <b-nav-item><router-link to="/" class="color-text">Home</router-link></b-nav-item>
        <b-nav-item><router-link to="/about" class="color-text">About</router-link></b-nav-item>
      </b-navbar-nav>
    </b-navbar>
    <router-view/>
  </div>
</template>

<style scoped>
  .color-text{
    color: white;
  }
</style>
