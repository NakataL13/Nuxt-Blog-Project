<template>
  <footer>
    <div class="container mx-auto bg-gray-800 p-8 flex justify-evenly">
      <NuxtLink to="/"
        ><h1 class="font-bold text-gray-400 text-[1.4rem] mt-[2rem]">
          B<span class="text-[#4338CA]">P</span>
        </h1></NuxtLink>
      <nav class="flex">
          
        <div class="hidden sm:block sm:ml-6">
            
          <div class="flex flex-col mr-[8rem]">
              <h1 class="ml-[1rem] font-bold text-gray-400 text-[1.3rem]">Social</h1>
            <NuxtLink
              to="/"
              class="text-[#4338CA] text-[0.9rem] hover:bg-white hover:text-black px-3 py-2 rounded-md text-sm font-medium"
              >FB - @NLambev13</NuxtLink
            >
            <NuxtLink
              to="/"
              class="text-[#4338CA] text-[0.9rem] hover:bg-white hover:text-black px-3 py-2 rounded-md text-sm"
              >G - @NLamebev</NuxtLink
            >
          </div>
        </div>
      </nav>
    </div>
  </footer>
</template>
