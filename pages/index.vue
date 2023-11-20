<template>
  <div
    class="absolute top-1/2 left-1/2 -translate-y-1/2 -translate-x-1/2 p-3 text-center w-1/2"
  >
    <h1
      class="text-6xl font-extrabold leading-none tracking-tight text-transparent bg-clip-text bg-gradient-to-r to-emerald-600 from-sky-400 h-20"
    >
      Digital Smart Office
    </h1>
    <p class="mb-6 text-lg font-normal text-gray-500 lg:text-xl">
      Positive growth and tech-driven mindset behind your daily tasks
    </p>
    <div class="flex justify-center">
      <NuxtLink
        to="/desk"
        class="inline-flex items-center justify-center mx-3 px-5 py-3 text-base font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:ring-blue-300"
      >
        Desk Office
        <svg
          class="w-3.5 h-3.5 ms-2 rtl:rotate-180"
          aria-hidden="true"
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 14 10"
        >
          <path
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M1 5h12m0 0L9 1m4 4L9 9"
          />
        </svg>
      </NuxtLink>
      <NuxtLink
        to="/document"
        class="inline-flex items-center justify-center mx-3 px-5 py-3 text-gray-400 font-medium text-center border border-gray-400 rounded-lg hover:bg-gray-200 focus:ring-4 focus:ring-gray-300"
      >
        My Document
      </NuxtLink>
    </div>
  </div>
</template>
