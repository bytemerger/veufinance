<template>
  <div class="flex flex-col rounded-xl md:rounded border border-opacity-35 md:border-opacity-30 p-3 lg:w-1/4 md:w-1/2 md:mr-10 mt-3 md:mt-0">
    <div class="text-gray-500 md:text-gray-400 md:text-xs mb-1.5">#43256723</div>
    <div class="font-medium text-xl md:text-sm mb-1.5">App Store</div>
    <div class="text-gray-400 very-small-text mb-1.5">12 Jun 2021, 11:00pm</div>
    <div class="border-b border-opacity-30 mb-2.5"></div>
    <div class="flex items-center">
      <div class="font-semibold md:font-medium md:text-sm">$120,00</div>
      <div class="inline-block ml-9 md:ml-3"><i class="fas fa-arrow-down"></i></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "InvoiceCard"
}
</script>

<style scoped>
@media only screen and (min-width: 700px) {
  .very-small-text {
    font-size: 0.5em;
  }
}
</style>
