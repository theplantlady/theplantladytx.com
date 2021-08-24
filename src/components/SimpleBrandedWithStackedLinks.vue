<!-- This example requires Tailwind CSS v2.0+ -->
<template>
  <header class="bg-gray-100">
    <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8" aria-label="Top">
      <div class="w-full py-2 flex items-center justify-between border-b border-gray-500 lg:border-none">
        <div class="flex items-center">
          <a href="#">
            <span class="sr-only">Workflow</span>
            <img class="h-16 w-auto" src="https://firebasestorage.googleapis.com/v0/b/xsqrd-inc.appspot.com/o/ThePlantLadyText.png?alt=media&token=5237c0f6-08ad-4a36-bf70-f64e38158bd5" alt="" />
          </a>
          <div class="hidden ml-10 space-x-8 lg:block">
            <a v-for="link in navigation" :key="link.name" :href="link.href" class="text-base font-medium text-gray-800 hover:text-indigo-500">
              {{ link.name }}
            </a>
          </div>
        </div>
        <div class="ml-10 space-x-4">
          <a href="#" class="inline-block bg-gray-500 py-2 px-4 border border-transparent rounded-md text-base font-medium text-white hover:bg-opacity-75">Sign in</a>
          <a href="#" class="inline-block bg-white py-2 px-4 border border-transparent rounded-md text-base font-medium text-gray-600 hover:bg-indigo-50">Sign up</a>
        </div>
      </div>
      <div class="py-4 flex flex-wrap justify-center space-x-6 lg:hidden">
        <a v-for="link in navigation" :key="link.name" :href="link.href" class="text-base font-medium text-gray-800 hover:text-indigo-500">
          {{ link.name }}
        </a>
      </div>
    </nav>
  </header>
</template>

<script>
const navigation = [
  { name: 'Home', href: '#' },
  { name: 'About', href: '#' },
  { name: 'Services', href: '#' },
  { name: 'Gallery', href: '#' },
]

export default {
  setup() {
    return {
      navigation,
    }
  },
}
</script>