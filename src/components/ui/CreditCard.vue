<template>
 <div>
   <div class="rounded shadow-2xl">
     <div class="card rounded-t">
       <div class="p-5">
         <div class="flex justify-between mb-5">
           <div class="text-sm text-gray-300">Helen Spanks</div>
           <div class="inline-block text-gray-400"><i class="fas fa-wifi"></i></div>
         </div>
         <div class="text-2xl font-semibold text-gray-100 mb-4">$42,870,00</div>
       </div>
     </div>
     <div class="flex justify-around bg-blue-200 p-3 rounded-b">
       <div>
         <div class="small-text text-gray-400">Card number</div>
         <div class="text-xs text-gray-800">**** **** **** 1290</div>
       </div>
       <div>
         <div class="small-text text-gray-500">Date</div>
         <div class="text-xs text-gray-800">12/24</div>
       </div>
       <div>
         <div class="small-text text-gray-500">CVC</div>
         <div class="text-xs text-gray-800">189</div>
       </div>
       <div class="w-12 self-center">
         <img src="../../assets/visa.png" class="h-9 w-12" alt="visa_logo">
       </div>
     </div>
   </div>
 </div>
</template>

<script>
export default {
  name: "CreditCard"
}
</script>

<style scoped>
.card{
  background: #171c28;
}
.small-text{
  font-size: 0.6em;
}
</style>
