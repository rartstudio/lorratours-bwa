<template>
     <footer class="container font-style-one mt-48 pb-16 bg-two rounded-tr-3xl w-full flex flex-col md:flex-row relative">
      <form class="register-form mx-4 flex flex-col md:flex-row absolute bg-white py-6 px-4 rounded-xl right-0 md:mr-12">
        <div class="flex flex-col items-center md:items-start md:mr-6 mb-4 md:mb-0">
          <h5 class="text-left font-style-two text-xl font-semibold">Subscribe For Discount</h5>  
          <p class="text-sm text-gray-600">We never send you any spam</p>
        </div>
        <input class="bg-gray-200 py-2 pl-4 md:w-64" type="text" name="" id="" value="masayoshi@bwa.co.id">
        <button type="submit" class="mt-4 ml-0 md:ml-6 text-white uppercase py-2 px-8 bg-one">subscribe</button>
      </form>
      <div class="w-full md:w-4/12 px-4 md:pl-32 pt-24 md:pt-32 flex flex-col justify-start items-start">
        <img src="~assets/images/logo.png" class="mb-8">
        <p class="text-white">Travel the place you always <br/> dreaming about, easier</p>
      </div>
      <div class="w-full md:w-3/12 px-4 pt-8 md:pt-32 flex flex-col">
        <h4 class="text-white text-lg mb-6">Company</h4>
        <ul>
          <li>
            <nuxt-link to="/home" class="text-gray-600 mb-2 inline-block">Flight Partners</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/home" class="text-gray-600 mb-2 inline-block">Hotel Group</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/home" class="text-gray-600 mb-2 inline-block">Accomodations</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/home" class="text-gray-600 mb-2 inline-block">Packages</nuxt-link>
          </li>
        </ul>
      </div>
      <div class="w-full md:w-3/12 px-4 pt-8 md:pt-32 flex flex-col">
        <h4 class="text-white text-lg mb-6">Account</h4>
        <ul>
          <li>
            <nuxt-link to="/home" class="text-gray-600 mb-2 inline-block">Refund Policy</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/home" class="text-gray-600 mb-2 inline-block">Setting</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/home" class="text-gray-600 mb-2 inline-block">Terms & Conditions</nuxt-link>
          </li>
        </ul>
      </div>
      <div class="w-full md:w-3/12 px-4 pt-8 md:pt-32 flex flex-col">
        <h4 class="text-white text-lg mb-6">Fast Response</h4>
        <p class="text-gray-600 mb-2">M Building No.11</p>
        <p class="text-gray-600 mb-2">cs@lorra.co.id</p>
        <p class="text-gray-600 mb-2">+021 2208 1996 1993</p>
        <p class="text-gray-600 mb-2">@lorragroup</p>
      </div>
    </footer>
</template>

<script>
    export default {
        
    }
</script>

<style>
@media (max-width: 640px){
    .register-form {
        top:-150px;
        left:0px;
        @apply shadow-xl;
    }
}
@media (min-width: 1024px){
    .register-form {
        top:-50px;
    }
}
</style>