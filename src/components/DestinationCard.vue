<template>
    <div class="flex bg-white shadow-xl items-center rounded-lg overflow-hidden">
        <img class=" h-32 w-32 flex-shrink-0" :src="destination.imageUrl" :alt="destination.imageAlt">
        <div class="p-4">
            <h1 class="text-lg font-bold text-gray-900">{{destination.city}}</h1>
            <p class="text-md text-gray-700">${{destination.averagePrice}} / night average</p>
            <div class="mt-4 text-sm text-blue-700">
                <a href="#">Explore {{destination.propertyCount}} properties</a>                        
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'DestinationCard',
    props: ['destination'],
}
</script>