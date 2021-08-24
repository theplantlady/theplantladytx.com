<script setup>
import ButtonRepo from '@/components/ButtonRepo.vue'
import LeftAlignedWImageAndFloatingCard from '@/components/LeftAlignedWImageAndFloatingCard.vue'
import SimpleBrandedWithStackedLinks from '@/components/SimpleBrandedWithStackedLinks.vue'

</script>

<template>
  <div>
    <header class="bg-white shadow" v-if="$route.meta.title">
    <SimpleBrandedWithStackedLinks />
      <!-- <div class="max-w-7xl mx-auto py-6 px-4 sm:px-6 lg:px-8">
        <h1 class="text-3xl font-bold leading-tight text-gray-900">{{ $route.meta.title }}</h1>
      </div> -->
        <LeftAlignedWImageAndFloatingCard />
    </header>
    <main>
      <router-view/>
    </main>
  </div>
</template>
