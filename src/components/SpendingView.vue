<template>
  <div>
    <div class="text-2xl font-semibold text-gray-800">My Spending</div>
    <div class="text-xs text-gray-500 mt-2.5">You can see the details of all your expenditures here. You can choose by month and manage</div>
    <div class="text-xl font-semibold mt-7 text-gray-800">
      $9,880,00
    </div>
    <div class="float-right flex rounded border border-gray-300 text-gray-500 pl-2 pr-2 items-center justify-around">
      <button>month</button>
      <div class="inline-block pl-2"><i class="fas fa-caret-down"></i></div>
    </div>
    <div class="mt-6 w-full mb-8">
     <img src="../assets/chart.png" class="w-full h-44" alt="chart">
    </div>
    <div>
      <div class="text-2xl mb-1.5 font-semibold text-gray-800">Invoices</div>
      <div class="flex justify-between mb-5">
        <div class="text-xs text-gray-400">Cernbank.inc 280, 550 street 12/3 man, London</div>
        <div class=" flex pr-1.5">
          <div class="inline-block mr-1.5"><i class="fas fa-chevron-circle-left"></i></div>
          <div class="inline-block"><i class="fas fa-chevron-circle-right"></i></div>
        </div>
      </div>
      <div class="flex w-56 overflow-x-auto masked">
        <div class="flex flex-col rounded border border-opacity-30 p-3 lg:w-1/4 md:w-1/2 mr-10">
          <div class="text-gray-400 text-xs mb-1.5">#43256723</div>
          <div class="font-medium text-sm mb-1.5">App Store</div>
          <div class="text-gray-400 very-small-text mb-1.5">12 Jun 2021, 11:00pm</div>
          <div class="border-b border-opacity-30 mb-2.5"></div>
          <div class="flex items-center">
            <div class="font-medium text-sm">$120,00</div>
            <div class="inline-block ml-3"><i class="fas fa-arrow-down"></i></div>
          </div>
        </div>
        <div class="flex flex-col rounded border border-opacity-30 p-3 lg:w-1/4 md:w-1/2 mr-10">
          <div class="text-gray-400 text-xs mb-1.5">#43256723</div>
          <div class="font-medium text-sm mb-1.5">App Store</div>
          <div class="text-gray-400 very-small-text mb-1.5">12 Jun 2021, 11:00pm</div>
          <div class="border-b border-opacity-30 mb-2.5"></div>
          <div class="flex items-center">
            <div class="font-medium text-sm">$120,00</div>
            <div class="inline-block ml-3"><i class="fas fa-arrow-down"></i></div>
          </div>
        </div>
        <div class="flex flex-col rounded border border-opacity-30 p-3 lg:w-1/4 md:w-1/2 mr-10">
          <div class="text-gray-400 text-xs mb-1.5">#43256723</div>
          <div class="font-medium text-sm mb-1.5">App Store</div>
          <div class="text-gray-400 very-small-text mb-1.5">12 Jun 2021, 11:00pm</div>
          <div class="border-b border-opacity-30 mb-2.5"></div>
          <div class="flex items-center">
            <div class="font-medium text-sm">$120,00</div>
            <div class="inline-block ml-3"><i class="fas fa-arrow-down"></i></div>
          </div>
        </div>
        <div class="flex flex-col rounded border border-opacity-30 p-3 lg:w-1/4 md:w-1/2 mr-10">
          <div class="text-gray-400 text-xs mb-1.5">#43256723</div>
          <div class="font-medium text-sm mb-1.5">App Store</div>
          <div class="text-gray-400 very-small-text mb-1.5">12 Jun 2021, 11:00pm</div>
          <div class="border-b border-opacity-30 mb-2.5"></div>
          <div class="flex items-center">
            <div class="font-medium text-sm">$120,00</div>
            <div class="inline-block ml-3"><i class="fas fa-arrow-down"></i></div>
          </div>
        </div>
        <div class="flex flex-col rounded border border-opacity-30 p-3 lg:w-1/4 md:w-1/2 mr-10">
          <div class="text-gray-400 text-xs mb-1.5">#43256723</div>
          <div class="font-medium text-sm mb-1.5">App Store</div>
          <div class="text-gray-400 very-small-text mb-1.5">12 Jun 2021, 11:00pm</div>
          <div class="border-b border-opacity-30 mb-2.5"></div>
          <div class="flex items-center">
            <div class="font-medium text-sm">$120,00</div>
            <div class="inline-block ml-3"><i class="fas fa-arrow-down"></i></div>
          </div>
        </div>
        <div class="flex flex-col rounded border border-opacity-30 p-3 lg:w-1/4 md:w-1/2 mr-10">
          <div class="text-gray-400 text-xs mb-1.5">#43256723</div>
          <div class="font-medium text-sm mb-1.5">App Store</div>
          <div class="text-gray-400 very-small-text mb-1.5">12 Jun 2021, 11:00pm</div>
          <div class="border-b border-opacity-30 mb-2.5"></div>
          <div class="flex items-center">
            <div class="font-medium text-sm">$120,00</div>
            <div class="inline-block ml-3"><i class="fas fa-arrow-down"></i></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SpendingView"
}
</script>

<style scoped>
.very-small-text{
  font-size: 0.5em;
}
.masked{
/*
  -webkit-mask-image: -webkit-gradient(linear,left 20%,left bottom,from(black),to(rgba(0,0,0,0)))
*/
  mask-image: linear-gradient(to right, black 80%, transparent);
}
::-webkit-scrollbar {
  width: 0;
  background: transparent;
}
@media only screen and (min-width: 900px) {
  .masked{
    width:45rem;
  }
}
</style>
