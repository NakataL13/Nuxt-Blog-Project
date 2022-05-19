<template>
  <div class="container mx-auto bg-gray-800 p-8 flex justify-between">
    <NuxtLink to="/"><h1 class="font-bold text-gray-400 text-[1.4rem]">
      Blog <span class="text-[#4338CA]">Page</span>
    </h1></NuxtLink>
      <nav class="nav-obj">
    <div class="hidden sm:block sm:ml-6">
      <div class="flex space-x-4">
                <NuxtLink
          to="/"
          class="text-[#4338CA] text-[1.3rem] hover:bg-white hover:text-black px-3 py-2 rounded-md text-sm font-medium"
          >Home</NuxtLink
        >
        <NuxtLink
          to="/posts"
          class="text-[#4338CA] text-[1.3rem] hover:bg-white hover:text-black px-3 py-2 rounded-md text-sm"
          >Posts</NuxtLink
        >
      </div>
    </div>
  </nav>
  </div>

</template>
