<template>
  <div class="flex">
    <div class="h-screen w-400px py-10 bg-base text-white">
      <span class="block ml-4 text-2xl font-bold">Growfit Headless CMS</span>
      <div class="flex items-center mt-10 ml-4">
        <span class="block text-xs whitespace-nowrap">コンテンツ</span>
        <div class="h-0 w-full ml-2 border-t border-dashed"></div>
      </div>

      <NuxtLink class="flex items-center w-full mt-5 p-4 rounded-lg" :class="{ 'bg-primary': $route.name === 'news' }"
        to="/news">
        <span class="material-icons block">article</span>
        <span class="block ml-4">ニュース</span>
      </NuxtLink>
      <NuxtLink class="flex items-center w-full mt-1 p-4 rounded-lg" :class="{ 'bg-primary': $route.name === 'sample' }"
        to="/sample">
        <span class="material-icons block">face</span>
        <span class="block ml-4">サンプル</span>
      </NuxtLink>
    </div>

    <main>
      <Nuxt />
    </main>
  </div>
</template>