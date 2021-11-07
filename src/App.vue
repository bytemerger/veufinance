<template>
  <div id="app" class="container mx-0 font-dm-sans">
    <div class="hidden md:flex">
      <side-bar class="flex-grow-0"></side-bar>
      <div class="border-l border-opacity-25"></div>
      <main class="flex-grow ml-14">
        <TheHeader></TheHeader>
        <div class="flex mt-9">
          <credit-view></credit-view>
          <div class="border-l  border-opacity-25 flex-grow-0 ml-7 mr-8"></div>
          <spending-view class="w-4/6"></spending-view>
        </div>
      </main>
    </div>
    <div class="md:hidden m-6">
      <MobileHeader>{{ view === 'spending' ? 'My Spending' : 'Credit Card' }}</MobileHeader>
      <div class="text-3xl mt-9 font-medium text-gray-900"> {{view === 'spending' ? '$9,888,00' : 'Hello Helen 👋'}}</div>
      <div class="mt-8 text-sm" :class="[ view === 'spending' ? 'hidden' : '']">
        <ul class="flex list-none text-xl">
          <li class="border-b pr-5 lg:pr-8 pb-2 border-opacity-30 active">Budget</li>
          <li class="border-b pr-5 lg:pr-8 pb-2 border-opacity-30 text-gray-500">Spending</li>
          <li class="border-b pr-5 lg:pr-8 pb-2 border-opacity-30 text-gray-500">Balance</li>
          <li class="border-b pr-5 lg:pr-8 pb-2 border-opacity-30 text-gray-500">Value</li>
        </ul>
      </div>
      <div class="mt-8 text-sm" :class="[ view === 'spending' ? '' : 'hidden']">
        <ul class="flex list-none text-xl">
          <li class="border-b pr-5 lg:pr-8 pb-2 border-opacity-30 active">Month</li>
          <li class="border-b pr-5 lg:pr-8 pb-2 border-opacity-30 text-gray-500">Weekly</li>
          <li class="border-b pr-5 lg:pr-8 pb-2 border-opacity-30 text-gray-500">Daily</li>
        </ul>
      </div>
      <spending-view></spending-view>
      <div class="masked" :class="[ view === 'spending' ? 'hidden' : '']">
        <credit-card v-for="n in 4" :light="n%2 === 0" :key="n" :mobile="true" class="mt-8 rounded-2xl"></credit-card>
      </div>
    </div>
  </div>
</template>

<script>

import SideBar from "./components/layout/SideBar";
import TheHeader from "./components/layout/TheHeader";
import CreditView from "./components/CreditView";
import SpendingView from "./components/SpendingView";
import MobileHeader from "./components/layout/MobileHeader";
import CreditCard from "./components/ui/CreditCard";
export default {
  name: 'App',
  components: {
    CreditCard,
    MobileHeader,
    SpendingView,
    CreditView,
    TheHeader,
    SideBar

  },
  data(){
    return{
      view: 'spending'
    }
  }
}
</script>

<style>
.active{
  position: relative;
}
.active::before {
  content: '';
  display: block;
  position: absolute;
  bottom: 0;
  width: 75%;
  left: 0;
  border-top: 1px solid black;
}
</style>
