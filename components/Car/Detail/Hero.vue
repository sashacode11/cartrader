<script setup>
const props = defineProps({
  car: Object
})
</script>

<template>
    <div class="mt-10">
        <NuxtImg :src="car.url" alt="" />
        <h1 class="mt-10 text-4xl">{{car.name}}</h1>
        <div class="tex-slate-500 flex text-lg mt-3 border-b pb-5 justify-between">
            <div class="flex">
            <p class="mr-3">{{car.seats}}</p>
            <p class="mr-2">|</p>
            <p class="mr-2">{{car.miles}}</p>
            </div>
            <div>
            <p class="font-bold text-xl">{{car.price}}</p>
            </div>
        </div>
    </div>
</template>