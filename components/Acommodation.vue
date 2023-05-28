<template>
  <section class="pt-[88px] md:px-[80px]">
    <div class="max-md:px-5">
      <h3 class="font-[700] leading-[28.13px] text-[24px] text-[#484848]">
        Akomodasi Airbnb Plus
      </h3>
      <p class="mt-[8px] font-light leading-[19px] text-[#484848] text-[16px]">
        Pilihan akomodasi diperiksa sesuai dengan kriteria kualitas dan desain
      </p>
    </div>
    <div
      class="mt-[24px] h-[301px] acommodation rounded-4px pt-[65.87px] pb-[131.87px] flex items-center flex-col"
    >
      <img
        src="~/assets/img/big-logo.png"
        class="w-[104.5px] h-[112.27px] object-cover"
        alt="AIRBNB"
      />
      <NuxtLink
        to="/acommodation"
        class="mt-[37.87px] hover:scale-x-110 transition-all ease"
      >
        <div
          class="bg-white py-[16px] pl-[24px] pr-[40px] rounded-[4px] font-bold text-[10px] leading-[12px] text-[#484848] uppercase relative"
        >
          <span>Temukan Akomodasi</span>
          <svg
            class="absolute top-[17px] right-[16px]"
            width="6"
            height="10"
            viewBox="0 0 6 10"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path d="M1 1L5 5L1 9" stroke="#484848" stroke-linecap="round" />
          </svg>
        </div>
      </NuxtLink>
    </div>
  </section>
</template>

<style scope>
.acommodation {
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.15), rgba(0, 0, 0, 0.15)),
    url(~/assets/img/acommodation.png), #c4c4c4;
  background-position: center;
  background-size: cover;
}
</style>
