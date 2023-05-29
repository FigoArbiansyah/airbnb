<template>
  <section class="md:px-[80px] px-5 pt-[88px]">
    <div>
      <h3 class="font-[700] leading-[28.13px] text-[24px] text-[#484848]">
        Explorer Airbnb
      </h3>
    </div>
    <div class="mt-[24px] flex gap-x-[16px] max-md:flex-wrap max-md:gap-y-8">
      <NuxtLink
        v-for="data in dataKategori"
        :to="`acommodation/${data.nama.toLowerCase()}`"
        class="category-card border w-full md:w-[391px] md:h-[85px] h-[100px] bg-white rounded-[12px] flex items-center overflow-hidden"
      >
        <div class="md:w-[121px] w-1/3 h-full relative bg-black">
          <img
            :src="`${data.img}`"
            class="object-cover w-full h-full opacity-90"
            alt=""
          />
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="#fff"
            class="w-6 h-6 absolute top-[50%] left-[50%] -translate-y-[50%] -translate-x-[50%] z-50"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              :d="data.iconPath"
            />
          </svg>
        </div>
        <div class="pl-[24px] py-[33px]">
          <p class="text-[16px] leading-[18.75px] text-[#484848]">
            {{ data.nama }}
          </p>
        </div>
      </NuxtLink>
    </div>
  </section>
</template>

<script setup>
import explorer1 from "~/assets/img/explorer1.png";
import explorer2 from "~/assets/img/explorer2.png";
import explorer3 from "~/assets/img/explorer3.png";

console.log("Halo")

const dataKategori = [
  {
    id: 1,
    nama: "Perumahan",
    img: explorer1,
    slug: "perumahan",
    iconPath:
      "M8.25 21v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21m0 0h4.5V3.545M12.75 21h7.5V10.75M2.25 21h1.5m18 0h-18M2.25 9l4.5-1.636M18.75 3l-1.5.545m0 6.205l3 1m1.5.5l-1.5-.5M6.75 7.364V3h-3v18m3-13.636l10.5-3.819",
  },
  {
    id: 2,
    nama: "Pengalaman",
    img: explorer2,
    slug: "pengalaman",
    iconPath:
      "M9.813 15.904L9 18.75l-.813-2.846a4.5 4.5 0 00-3.09-3.09L2.25 12l2.846-.813a4.5 4.5 0 003.09-3.09L9 5.25l.813 2.846a4.5 4.5 0 003.09 3.09L15.75 12l-2.846.813a4.5 4.5 0 00-3.09 3.09zM18.259 8.715L18 9.75l-.259-1.035a3.375 3.375 0 00-2.455-2.456L14.25 6l1.036-.259a3.375 3.375 0 002.455-2.456L18 2.25l.259 1.035a3.375 3.375 0 002.456 2.456L21.75 6l-1.035.259a3.375 3.375 0 00-2.456 2.456zM16.894 20.567L16.5 21.75l-.394-1.183a2.25 2.25 0 00-1.423-1.423L13.5 18.75l1.183-.394a2.25 2.25 0 001.423-1.423l.394-1.183.394 1.183a2.25 2.25 0 001.423 1.423l1.183.394-1.183.394a2.25 2.25 0 00-1.423 1.423z",
  },
  {
    id: 3,
    nama: "Petualangan",
    img: explorer3,
    slug: "petualangan",
    iconPath:
      "M14.25 6.087c0-.355.186-.676.401-.959.221-.29.349-.634.349-1.003 0-1.036-1.007-1.875-2.25-1.875s-2.25.84-2.25 1.875c0 .369.128.713.349 1.003.215.283.401.604.401.959v0a.64.64 0 01-.657.643 48.39 48.39 0 01-4.163-.3c.186 1.613.293 3.25.315 4.907a.656.656 0 01-.658.663v0c-.355 0-.676-.186-.959-.401a1.647 1.647 0 00-1.003-.349c-1.036 0-1.875 1.007-1.875 2.25s.84 2.25 1.875 2.25c.369 0 .713-.128 1.003-.349.283-.215.604-.401.959-.401v0c.31 0 .555.26.532.57a48.039 48.039 0 01-.642 5.056c1.518.19 3.058.309 4.616.354a.64.64 0 00.657-.643v0c0-.355-.186-.676-.401-.959a1.647 1.647 0 01-.349-1.003c0-1.035 1.008-1.875 2.25-1.875 1.243 0 2.25.84 2.25 1.875 0 .369-.128.713-.349 1.003-.215.283-.4.604-.4.959v0c0 .333.277.599.61.58a48.1 48.1 0 005.427-.63 48.05 48.05 0 00.582-4.717.532.532 0 00-.533-.57v0c-.355 0-.676.186-.959.401-.29.221-.634.349-1.003.349-1.035 0-1.875-1.007-1.875-2.25s.84-2.25 1.875-2.25c.37 0 .713.128 1.003.349.283.215.604.401.96.401v0a.656.656 0 00.658-.663 48.422 48.422 0 00-.37-5.36c-1.886.342-3.81.574-5.766.689a.578.578 0 01-.61-.58v0z",
  },
];
</script>

<style scope>
.category-card {
  transition: all 0.3s ease;
}
.category-card:hover {
  transform: scale(1.02);
  filter: drop-shadow(0px 0px 15px rgba(0, 0, 0, 0.15));
}
</style>
