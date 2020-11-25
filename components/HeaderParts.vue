<template>
    <header class="header font-style-one py-6 md:pt-8 flex items-center justify-between">
          <img src="~assets/images/logo.png" class="px-4 md:px-0 ">
          <ul class="hidden md:flex justify-between items-center">
            <li>
              <nuxt-link to="/" class="text-black md:text-white opacity-75 px-4 link">Landing</nuxt-link>
            </li>
            <li>
              <nuxt-link to="/home" class="text-black md:text-white opacity-75 px-6 link">Packages</nuxt-link>
            </li>
            <li>
              <nuxt-link to="/home" class="text-black md:text-white opacity-75 px-6 link">Stories</nuxt-link>
            </li>
            <li>
              <nuxt-link to="/home" class="text-black md:text-white opacity-75 px-6 link">Product</nuxt-link>
            </li>
            <li>
              <nuxt-link to="/home" class="text-black md:text-white opacity-75 px-6 link">Gallery</nuxt-link>
            </li>
            <li>
              <nuxt-link to="/home" class="text-black md:text-white opacity-75 px-6 link border-l py-4">Sign Up</nuxt-link>
            </li>
            <li>
              <nuxt-link to="/home" class="text-black md:text-white opacity-75 px-6 link">Login</nuxt-link>
            </li>
          </ul>
        </header>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

</style>