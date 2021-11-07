<template>
  <div class="flex justify-between mt-3 items-center">
    <div class="inline-block rounded-md px-2 py-1 shadow-sm border text-gray-500">
      <i class="fas fa-bars"></i>
    </div>
    <div class="inline-block px-1 m-3 font-medium text-xl">
      <slot></slot>
    </div>
    <div class="inline-block rounded-md px-2 py-1 shadow-sm border text-gray-500 tx-sm">
      <i class="fas fa-search"></i>
    </div>
  </div>
</template>

<script>
export default {
  name: "MobileHeader"
}
</script>

<style scoped>

</style>
