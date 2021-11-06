<template>
  <div id="app" class="container mx-0 font-dm-sans">
    <div class="flex">
      <side-bar class="flex-grow-0"></side-bar>
      <div class="border-l border-opacity-25"></div>
      <main class="flex-grow ml-14">
        <Header></Header>
        <div class="flex mt-9">
          <credit-view></credit-view>
          <div class="border-l  border-opacity-25 flex-grow-0 ml-7 mr-8"></div>
          <spending-view class="w-4/6"></spending-view>
        </div>
      </main>
    </div>
  </div>
</template>

<script>

import SideBar from "./components/layout/SideBar";
import Header from "./components/layout/Header";
import CreditView from "./components/CreditView";
import SpendingView from "./components/SpendingView";
export default {
  name: 'App',
  components: {
    SpendingView,
    CreditView,
    Header,
    SideBar

  }
}
</script>

<style>

</style>
