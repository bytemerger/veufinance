<template>
  <div>
    <div class="text-2xl font-semibold text-gray-800">Credit Card</div>
    <div class="text-xs text-gray-500 mt-2.5">You can find all the information about your credit card here</div>
    <div class="mt-8 text-sm">
      <ul class="flex list-none">
        <li class="border-b pr-5 lg:pr-8 pb-2 border-opacity-25 active">Budget</li>
        <li class="border-b pr-5 lg:pr-8 pb-2 border-opacity-25 text-gray-600">Spending</li>
        <li class="border-b pr-5 lg:pr-8 pb-2 border-opacity-25 text-gray-600">Balance</li>
        <li class="border-b pr-5 lg:pr-8 pb-2 border-opacity-25 text-gray-600">Value</li>
      </ul>
    </div>
    <div class="card-holder masked overflow-x-auto h-120">
      <credit-card v-for="n in 4" :light="n%2 === 0" :key="n" class="mt-8"></credit-card>
    </div>
  </div>
</template>

<script>
import CreditCard from "./ui/CreditCard";
export default {
  name: "CreditView",
  components: {CreditCard}
}
</script>

<style scoped>
@media only screen and (min-width: 900px) {
  .masked{
    /*
      -webkit-mask-image: -webkit-gradient(linear,left 20%,left bottom,from(black),to(rgba(0,0,0,0)))
    */
    mask-image: linear-gradient(to bottom, black 80%, white);
  }
}
::-webkit-scrollbar {
  width: 0;
  background: transparent;
}
.h-120{
  height: 28rem;
}
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
