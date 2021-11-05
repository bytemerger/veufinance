<template>
  <div id="app" class="container mx-0">
    <div class="flex">
      <side-bar class="flex-grow-0"></side-bar>
      <main class="flex-grow">
        <Header></Header>
      </main>
    </div>
  </div>
</template>

<script>

import SideBar from "./components/layout/SideBar";
import Header from "./components/layout/Header";
export default {
  name: 'App',
  components: {
    Header,
    SideBar

  }
}
</script>

<style>

</style>
