<template>
  <div>
    <div class="hero w-full max-h-screen h-screen min-h-screen relative">
      <div class="max-h-screen h-screen min-h-screen absolute inset-0 opacity-50 bg-black z-20"></div>
      <img src="~assets/images/image 5.png" class="object-cover w-full absolute inset-0 z-10 max-h-screen h-screen min-h-screen">
      <div class="relative z-30 container mx-auto">
        <HeaderParts/>
        <div class="w-full flex flex-col md:flex-row justify-between">
          <div class="flex flex-col items-center md:items-start w-full md:w-6/12 mt-16 md:mt-32">
            <h1 class="text-5xl font-semibold tracking-wide text-white font-style-two">Find Your True <br/> Adventure Soul</h1>
            <p class="text-center md:text-left text-lg text-white font-style-one mt-6 opacity-75">Time to reconstruct your imagination <br>
                with what we provide special just for you
            </p>
            <div class="hidden md:flex items-center mt-10">
              <div class="w-3 h-3 rounded-full bg-white mr-4"></div>
              <div class="w-3 h-3 rounded-full bg-yellow-500 mr-4"></div>
              <div class="w-3 h-3 rounded-full bg-white mr-4"></div>
              <div class="w-3 h-3 rounded-full bg-white mr-4"></div>
              <div class="w-3 h-3 rounded-full bg-white mr-4"></div>
            </div>
          </div>
          <div class="relative w-full md:w-4/12 font-style-one">
            <div class="relative">
              <form class="transform translate-y-24 flex flex-col bg-white pb-40 p-8 md:p-8">
                <div class="w-full flex flex-col mb-4">
                  <label class="text-gray-600 mb-1" for="">Activity</label>
                  <input class="bg-gray-200 px-4 py-4" type="text" value="Nature and Adventure"/>
                </div>
                <div class="w-full flex flex-col mb-4">
                  <label class="text-gray-600 mb-1" for="">Location</label>
                  <input class="bg-gray-200 px-4 py-4" type="text" value="Bandung, Indonesia"/>
                </div>
                <div class="w-full flex flex-col mb-4">
                  <label class="text-gray-600 mb-1" for="">Date</label>
                  <input class="bg-gray-200 px-4 py-4" type="text" value="Friday, August 8, 2021"/>
                </div>
                <div class="w-full flex flex-col mb-4">
                  <div class="flex">
                    <div class="w-1/2 flex flex-col mb-4 mr-2">
                      <label class="text-gray-600 mb-1" for="">Adult</label>
                      <input class="bg-gray-200 px-4 py-4" type="text" value="12 People"/>
                    </div>
                    <div class="w-1/2 flex flex-col mb-4">
                      <label class="text-gray-600 mb-1" for="">Kid</label>
                      <input class="bg-gray-200 px-4 py-4" type="text" value="3 People"/>
                    </div>
                  </div>
                </div>
                <button class="w-full bg-one text-white py-4" type="submit">Explore Now</button>
              </form>
              <div class="hidden md:block form-border absolute border border-black inset-0"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="w-full mt-48 flex items-center flex-col justify-center container mx-auto">
      <h5 class="font-style-one text-xl text-orange-600 uppercase mb-2" data-aos="slide-up" data-aos-duration="500">your dreams</h5>
      <h1 class="font-style-two text-3xl text-center font-semibold mb-12" data-aos="slide-up" data-aos-duration="750">We Have Few Packages <br> With Friendly Price</h1>
      <TourItem/>
    </div>
    <ReviewParts/>
    <FooterParts/>
  </div>
</template>

<script>
export default {}
</script>

<style>
.nuxt-link-active {
  color: #fff !important; 
  opacity: 1 !important ;
}
.font-style-one {
  font-family: 'Lato', sans-serif;
}
.font-style-two {
  font-family: 'Lora', serif;
}
.bg-one {
  background: #539592;
}
.bg-two {
  background: #192E46;
}
.link:hover {
  @apply transition-all duration-200;
  color: #fff;
  opacity: 1;
}
.form-border {
    top: 70px;
    bottom: -120px;
    left: -25px;
    right: 30px;
    z-index: -1;
}
</style>
