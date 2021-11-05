<template>
  <div>
    <div class="text-3xl">Credit Card</div>
    <div class="text-xs text-gray-500 mt-2.5">You can find all the information about your credit card here</div>
    <div class="mt-8 text-sm">
      <ul class="flex list-none">
        <li class="border-b pr-8 pb-2 border-opacity-25">Budget</li>
        <li class="border-b pr-8 pb-2 border-opacity-25">Spending</li>
        <li class="border-b pr-8 pb-2 border-opacity-25">Balance</li>
        <li class="border-b pr-8 pb-2 border-opacity-25">Value</li>
      </ul>
    </div>
    <credit-card class="mt-8"></credit-card>
    <credit-card class="mt-4"></credit-card>
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

</style>
