<template>
  <div>
    <div class=" hidden text-2xl font-semibold text-gray-800 md:block">My Spending</div>
    <div class="hidden text-xs text-gray-500 mt-2.5 md:block">You can see the details of all your expenditures here. You can choose by month and manage</div>
    <div class="hidden text-xl font-semibold mt-7 text-gray-800 md:block">
      $9,880,00
    </div>
    <div class="hidden md:flex float-right rounded border border-gray-300 text-gray-500 pl-2 pr-2 items-center justify-around">
      <button>month</button>
      <div class="inline-block pl-2"><i class="fas fa-caret-down"></i></div>
    </div>
    <div class="h-54 pt-4">
      <spending-chart class="h-52 mt-7 mb-5"></spending-chart>
    </div>
    <div class="mt-12 md:mt-0">
      <div class="text-3xl md:text-2xl mb-1.5 font-medium md:font-semibold text-gray-800">Invoices</div>
      <div class="flex justify-between mb-5">
        <div class="md:text-xs text-gray-400">Cernbank.inc 280, 550 street 12/3 man, London</div>
        <div class="hidden md:flex pr-1.5">
          <div class="inline-block mr-1.5"><i class="fas fa-chevron-circle-left"></i></div>
          <div class="inline-block"><i class="fas fa-chevron-circle-right"></i></div>
        </div>
      </div>
      <div class="flex flex-wrap justify-between md:justify-start md:flex-nowrap md:w-56 md:overflow-x-auto masked">
        <invoice-card v-for="n in 6" :key="n"></invoice-card>
      </div>
    </div>
  </div>
</template>

<script>
import SpendingChart from "./ui/SpendingChart";
import InvoiceCard from "./ui/InvoiceCard";
export default {
  name: "SpendingView",
  components: {InvoiceCard, SpendingChart}
}
</script>

<style scoped>
@media only screen and (min-width: 700px) {
  .masked {
    /*
    -webkit-mask-image: -webkit-gradient(linear,left 20%,left bottom,from(black),to(rgba(0,0,0,0)))
  */
    mask-image: linear-gradient(to right, black 80%, transparent);
  }

  ::-webkit-scrollbar {
    width: 0;
    background: transparent;
  }
}
@media only screen and (min-width: 900px) {
  .masked{
    width:45rem;
  }
}
</style>
