<template>
    <header :class="[ToggleMenu ? 'pb-18' : '','header font-style-one py-6 md:pt-8 flex items-center justify-between px-4']">
          <div :class="[ToggleMenu ? 'fixed z-50 -mx-4 px-4 pt-9' : '','flex justify-between w-full md:w-3/12 items-center']">
            <img src="~assets/images/logo.png" class="px-0 relative z-50">
            <div class="flex md:hidden">
                <button @click="setToggleMenu(ToggleMenu)"
                    :class="['toggle z-50', ToggleMenu ? 'active' : '']"
                    >
                </button>
            </div>
          </div>
          <ul :class="['fixed inset-0 bg-green-400  md:bg-transparent md:relative md:opacity-100 md:visible pt-24 md:pt-0 transition-all duration-200  overflow-hidden md:flex justify-between items-center',
          ToggleMenu ? 'opacity-100 visible z-40' : 'opacity-0 invisible']">
            <li class="my-4 md:my-0">
              <nuxt-link to="/" class="text-black text-xl md:text-base md:text-white opacity-75 px-4 md:px-6 link">Landing</nuxt-link>
            </li>
            <li class="my-4 md:my-0">
              <nuxt-link to="/home" class="text-black text-xl md:text-base md:text-white opacity-75 px-4 md:px-6 link">Packages</nuxt-link>
            </li>
            <li class="my-4 md:my-0">
              <nuxt-link to="/home" class="text-black text-xl md:text-base md:text-white opacity-75 px-4 md:px-6 link">Stories</nuxt-link>
            </li>
            <li class="my-4 md:my-0">
              <nuxt-link to="/home" class="text-black text-xl md:text-base md:text-white opacity-75 px-4 md:px-6 link">Product</nuxt-link>
            </li>
            <li class="my-4 md:my-0">
              <nuxt-link to="/home" class="text-black text-xl md:text-base md:text-white opacity-75 px-4 md:px-6 link">Gallery</nuxt-link>
            </li>
            <li class="my-4 md:my-0">
              <nuxt-link to="/home" class="text-black text-xl md:text-base md:text-white opacity-75 px-4 md:px-6 link border-l py-4">Sign Up</nuxt-link>
            </li>
            <li class="my-4 md:my-0">
              <nuxt-link to="/home" class="text-black text-xl md:text-base md:text-white opacity-75 px-4 md:px-6 link">Login</nuxt-link>
            </li>
          </ul>
        </header>
</template>

<script>
    export default {
        data() {
          return {
            ToggleMenu: false
          }
        },
        methods: {
            setToggleMenu(toggle){
                return this.ToggleMenu = !toggle
            }
        },
    }
</script>

<style>
.pt-9 {
  padding-top:35px;
}
.pb-18 {
  padding-bottom: 60px;
}
.toggle {
    position: relative;
    width: 20px;
    height: 20px;
    z-index: 9999;
}
.toggle:focus {
    outline: none
}
.toggle:before,
.toggle:after{
    @apply right-0 absolute bg-gray-200 transition-all duration-200;
    content: "";
    height:3px;
    transform-origin:center;
}
.toggle:before{
    top:26%;
    width: 20px;
}
.toggle:after{
    top: 58%;
    width: 12px;
}
.toggle.active:before{
    transform: translateY(-50%) rotate(-45deg);
}
.toggle.active:after{
    transform: translateY(-50%) rotate(45deg);
}
.toggle.active:before, .toggle.active:after {
    width: 20px;
    top: 50%;
}
</style>