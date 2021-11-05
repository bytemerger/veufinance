<template>
  <div class="pt-3">
    <div class="flex justify-between items-center mb-2">
      <div class="flex items-center">
        <i class="fa fa-search text-gray-300 text-xl"></i>
        <input type="text" name="search" placeholder="Search something..." class="inline-block px-2 outline-none align-middle text-xs text-gray-400">
      </div>
      <div>
        <div class="inline-block rounded px-1 shadow-sm border m-3 text-gray-500">
          <i class="far fa-comment"></i>
        </div>
        <div class="inline-block rounded px-1 shadow-sm border m-3 text-gray-500">
          <i class="far fa-bell"></i>
        </div>
        <div class="inline-block rounded px-1 shadow-sm border m-3 text-gray-500">
          <i class="fas fa-bars"></i>
        </div>
      </div>
    </div>
    <div class="border-b  border-opacity-30"/>
  </div>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>

</style>
