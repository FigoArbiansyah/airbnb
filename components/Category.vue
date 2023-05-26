<template>
  <section class="md:px-[80px] px-5 pt-[88px]">
    <div>
      <h3 class="font-[700] leading-[28.13px] text-[24px] text-[#484848]">
        Explorer Airbnb
      </h3>
    </div>
    <div class="mt-[24px] flex gap-x-[16px] max-md:flex-wrap max-md:gap-y-8">
      <div
        class="category-card border w-full md:w-[391px] md:h-[85px] h-[100px] bg-white rounded-[12px] flex items-center overflow-hidden"
      >
        <div class="md:w-[121px] w-1/3 h-full object-cover">
          <img
            src="~/assets/img/explorer1.png"
            class="object-cover w-full h-full"
            alt=""
          />
        </div>
        <div class="pl-[24px] py-[33px]">
          <p class="text-[16px] leading-[18.75px] text-[#484848]">Logements</p>
        </div>
      </div>
      <div
        class="category-card border w-full md:w-[391px] md:h-[85px] h-[100px] bg-white rounded-[12px] flex items-center overflow-hidden"
      >
        <div class="md:w-[121px] w-1/3 h-full">
          <img
            src="~/assets/img/explorer2.png"
            class="object-cover w-full h-full"
            alt=""
          />
        </div>
        <div class="pl-[24px] py-[33px]">
          <p class="text-[16px] leading-[18.75px] text-[#484848]">
            Expériences
          </p>
        </div>
      </div>
      <div
        class="category-card border w-full md:w-[391px] md:h-[85px] h-[100px] bg-white rounded-[12px] flex items-center overflow-hidden"
      >
        <div class="md:w-[121px] w-1/3 h-full">
          <img
            src="~/assets/img/explorer3.png"
            class="object-cover w-full h-full"
            alt=""
          />
        </div>
        <div class="pl-[24px] py-[33px]">
          <p class="text-[16px] leading-[18.75px] text-[#484848]">Aventures</p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scope>
.category-card {
  transition: all 0.3s ease;
}
.category-card:hover {
  transform: scale(1.02);
  filter: drop-shadow(0px 0px 15px rgba(0, 0, 0, 0.15));
}
</style>
