<template>
  <div>
    <div class="text-3xl">My Spending</div>
    <div class="text-xs text-gray-500 mt-2.5">You can see the details of all your expenditures here. You can choose by month and manage</div>
    <div class="text-xl font-medium mt-7 text-gray-700">
      $9,880,00
    </div>
    <div class="float-right flex rounded border border-gray-300 text-gray-500 pl-2 pr-2 items-center justify-around">
      <button>month</button>
      <div class="inline-block pl-2"><i class="fas fa-caret-down"></i></div>
    </div>
    <div class="h-44">
      <spending-chart class="h-56"></spending-chart>
    </div>
<!--    <div class="mt-6 text-sm">
      <ul class="flex list-none">
        <li class="border-b pr-8 pb-2 border-opacity-25">Budget</li>
        <li class="border-b pr-8 pb-2 border-opacity-25">Spending</li>
        <li class="border-b pr-8 pb-2 border-opacity-25">Balance</li>
        <li class="border-b pr-8 pb-2 border-opacity-25">Value</li>
      </ul>
    </div>-->
  </div>
</template>

<script>
import SpendingChart from "./ui/SpendingChart";
export default {
  name: "SpendingView",
  components: {SpendingChart}
}
</script>

<style scoped>

</style>
