<template>
  <nav class="bg-red shadow-sm">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Flex container -->
      <div class="flex justify-between items-center h-18 pt-8 pb-5">
        <!-- Left side: Logo -->
        <div class="flex items-center">
          <NuxtLink class="flex text-xl font-bold text-gray-800 hover:text-gray-600 pr-5">
            My Logo
          </NuxtLink>
        </div>

        <!-- Centered Menu -->
        <div class="hidden sm:flex sm:space-x-8 justify-center w-full">
          <nav>
            <ul class="flex justify-center space-x-4 list-style-none">
              <li>
                <NuxtLink to="/homePage" class="px-2">home</NuxtLink>
              </li>
              <li>
                <NuxtLink to="/aboutPage" class="px-2">about</NuxtLink>
              </li>
              <li>
                <NuxtLink to="/contactPage" class="px-2">contact page</NuxtLink>
              </li>
              <li>
                <NuxtLink to="/servicePage" class="px-2">service page</NuxtLink>
              </li>
            </ul>
          </nav>
        </div>

        <!-- Right side: Login and Sign-up -->
        <div class="hidden sm:flex sm:items-center">
          <NuxtLink to="/servicePage">login</NuxtLink>
          <NuxtLink to="/servicePage" class="mx-4 px-5 py-1 bg-blue-600 rounded text-white">signup</NuxtLink>
        </div>

        <!-- Mobile menu button -->
        <div class="-mr-2 flex items-center sm:hidden">
          <button @click="toggleMenu">
            <svg
              class="h-6 w-6"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              aria-hidden="true"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>
          </button>
        </div>
      </div>

      <!-- Mobile menu -->
      <div v-if="isOpen" class="sm:hidden">
        <nav>
          <ul class="list-style-none pt-6">
            <li>
              <NuxtLink to="/homePage" class="px-2">home</NuxtLink>
            </li>
            <li>
              <NuxtLink to="/aboutPage" class="px-2">about</NuxtLink>
            </li>
            <li>
              <NuxtLink to="/contactPage" class="px-2">contact page</NuxtLink>
            </li>
            <li>
              <NuxtLink to="/servicePage" class="px-2">service page</NuxtLink>
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
    };
  },

  methods: {
    toggleMenu() {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>

