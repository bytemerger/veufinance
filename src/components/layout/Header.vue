<template>
  <div class="p-3">
    <div class="flex justify-between items-center mb-4">
      <div class="flex items-center ml-10">
        <i class="fa fa-search text-gray-300 text-xl"></i>
        <input type="text" name="search" placeholder="Search something..." class="inline-block px-2 outline-none align-middle text-xs text-gray-400">
      </div>
      <div>
        <div class="inline-block rounded px-1 shadow-sm border-2 m-3">
          <i class="far fa-comment"></i>
        </div>
        <div class="inline-block rounded px-1 shadow-sm border-2 m-3">
          <i class="far fa-bell"></i>
        </div>
        <div class="inline-block rounded px-1 shadow-sm border-2 m-3">
          <i class="fas fa-bars"></i>
        </div>
      </div>
    </div>
    <hr class="ml-10 h-0.5 bg-gray-50 border-0"/>
  </div>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>

</style>
