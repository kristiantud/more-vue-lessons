<template>
  <div>
    <router-link :to="{name: 'HomePage'}">Home</router-link>
    <!--benefit of this: we don't have to worry about messing up the routing when we change the actual route in the browser (e.g. /about to /about-us)-->
    <router-link to="/about">About</router-link>
    <!--this is more efficient than simply requesting a new html page, like we would in a href -->
  </div>
  <router-view />
  <h1>this is the footer, it will stay the same</h1>
</template>

<script setup>



</script>

<style>

</style>
