<template>
  <div class="bg-white p-4">
    <div class="container mx-auto flex flex-row justify-between">
      <div class="flex">
        <div class="text-3xl font-bold text-primary-900">
          <RouterLink to="/">Event</RouterLink>
        </div>
        <ul class="text-xl hidden md:flex gap-10 ml-16">
          <li
            :class="{
              'text-primary-500 underline': $route.path === '/',
              'text-primary-900': $route.path !== '/'
            }"
          >
            <RouterLink to="/" exact>Home</RouterLink>
          </li>
          <li
            :class="{
              'text-primary-500 underline': $route.path === '/about',
              'text-primary-900': $route.path !== '/about'
            }"
          >
            <RouterLink to="/about">About</RouterLink>
          </li>
        </ul>
      </div>
      <button
        class="text-xl font-semibold text-white bg-primary-400 hover:bg-primary-500 rounded-full w-24"
      >
        World
      </button>
    </div>
  </div>

  <RouterView />
</template>
