<template>
  <div id="app">
    <b-card title="Card Title" no-body>
    <b-card-header header-tag="nav">
      <b-nav  class="box-shadow">
        <b-nav-item to="/" >Home</b-nav-item>
        <b-nav-item to="/about">About</b-nav-item>
        <b-nav-item v-if="$auth.isAuthenticated" to="/profile" >Profile</b-nav-item>
      </b-nav>
    </b-card-header>
    <b-card-body class="text-center">
      <router-view />
    </b-card-body>
  </b-card>
    <!-- <div id="nav">
      <router-link >Home</router-link>|
      <router-link >About</router-link>|
      <router-link >Profile</router-link>
    </div> -->
    
  </div>
</template>

<script>
export default {

};
</script>

<style>
.box-shadow {
  box-shadow: rgba(0, 0, 0, 0.12) 0px 1px 3px, rgba(0, 0, 0, 0.24) 0px 1px 2px;
}
</style>