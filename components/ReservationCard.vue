<template>
  <div
    class="md:w-[391px] md:min-h-[508px] w-[350px] min-h-[467px] bg-white absolute left-[58px] top-[132px] z-40 pt-[32px] px-[24px] rounded-[4px] pb-[24px] card max-md:top-[50%] max-md:left-[50%] max-md:-translate-y-[50%] max-md:-translate-x-[50%]"
  >
    <h2 class="text-[32px] leading-[37.5px] text-[#484848]">
      Réservez des hébergements et des activités uniques.
    </h2>
    <form>
      <div class="mt-[24px]">
        <label
          for=""
          class="text-[#484848] font-[700] text-[12px] leading-[14px] uppercase"
          >Où</label
        >
        <input type="" :class="input_style" value="" placeholder="Partout" />
      </div>
      <div class="mt-[16px] flex">
        <div>
          <label
            for=""
            class="text-[#484848] font-[700] text-[12px] leading-[14px] uppercase"
            >Arrivée</label
          >
          <input
            type=""
            :class="input_style"
            value=""
            placeholder="jj/mm/aaaa"
          />
        </div>
        <div>
          <label
            for=""
            class="text-[#484848] font-[700] text-[12px] leading-[14px] uppercase"
            >Départ</label
          >
          <input
            type=""
            :class="input_style"
            value=""
            placeholder="jj/mm/aaaa"
          />
        </div>
      </div>
      <div class="mt-[16px]">
        <label
          for=""
          class="text-[#484848] font-[700] text-[12px] leading-[14px] uppercase"
          >Voyageurs</label
        >
        <input type="" :class="input_style" value="" placeholder="Voyageurs" />
      </div>
      <div class="mt-[24px] text-end">
        <button type="submit" @click="handleClick()" :class="button_style">
          Rechercher
        </button>
      </div>
    </form>
  </div>
</template>

<script setup>
const input_style =
  "w-full mt-[8px] block box-border bg-white border border-[#E3E3E3] rounded-[2px] pt-[16px] px-[16px] pb-[14px] outline-none focus:border-[#b3b3b3] transition-all ease placeholder:text-[#8F8F8F] placeholder:leading-[18.75px] placeholder:text-[16px] placeholder:font-[400]";

const button_style =
  "bg-[#FF5A5F] text-white font-[700] text-[16px] font-[18.75px] pt-[15px] pb-[14px] pl-[31px] pr-[32px] rounded-[4px]";

const handleClick = () => {
  document.querySelector(".text-end").style.animation =
    "button_clicked .7s ease";
};
</script>

<style scope>
@keyframes button_clicked {
  0% {
    transform: scaleY(1);
  }
  50% {
    transform: scaleY(0.9);
  }
  100% {
    transform: scaleY(1);
  }
}
</style>
