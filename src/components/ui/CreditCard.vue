<template>
   <div class="shadow-xl overflow-hidden border-l-2 border-r-2 border-t-2 border-gray-100">
     <div :class="[ light ? 'car-light' : 'card-dark']">
       <div class="p-5">
         <div class="flex justify-between mb-5">
           <div class="text-sm"  v-bind:class="[ light ? 'text-gray-800' : 'text-gray-300']" >Helen Spanks</div>
           <div class="inline-block text-gray-400" :class="[ light ? 'text-gray-800' : 'text-gray-400']"><i class="fas fa-wifi"></i></div>
         </div>
         <div class="text-2xl font-semibold mb-4" :class="[ light ? 'text-gray-800' : 'text-gray-100']">$42,870,00</div>
       </div>
     </div>
     <div class="flex justify-around p-3" :class="[ light ? 'bg-gray-50' : 'bg-blue-200']">
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
</template>

<script>
export default {
  name: "CreditCard",
  props:{
    light:{
      type: Boolean,
      required: true
    }
  }
}
</script>

<style scoped>
.card-dark{
  background: #171c28;
}
.card-light{
  background: #fafafa;
}
.small-text{
  font-size: 0.6em;
}
</style>
