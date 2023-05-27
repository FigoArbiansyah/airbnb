<template>
  <section class="md:px-[80px] pt-[88px] px-5">
    <div>
      <h3 class="font-[700] leading-[28.13px] text-[24px] text-[#484848]">
        Expériences très bien notées
      </h3>
      <p class="mt-[8px] font-light leading-[19px] text-[#484848] text-[16px]">
        Voyages de plusieurs jours organisés par des experts locaux avec
        activités, repas et logements compris
      </p>
    </div>
    <div
      class="mt-[24px] flex gap-x-[16px] max-md:overflow-x-auto max-md:w-auto max-md:flex-wrap max-md:justify-center max-md:gap-y-6"
    >
      <div v-for="data in dataTempat" class="md:w-[188px] w-full">
        <div class="w-full h-[240px] overflow-hidden">
          <img
            :src="data.gambar"
            class="h-full w-full object-cover rounded-[4px] hover:scale-110 cursor-pointer transition-all ease duration-500"
            alt=""
          />
        </div>
        <p
          class="text-[#767676] text-[10px] font-bold uppercase mt-2 leading-[11.72px]"
        >
          {{ data.wilayah }}
        </p>
        <h5 class="text-[16px] leading-[18.75px] font-bold mt-1">
          {{ data.deskripsi }}
        </h5>
        <p class="mt-2 text-sm leading-[21px] font-light text-[#484848]">
          Dari Rp. {{ data.harga.perOrang }} / orang - &nbsp; Rp.
          {{ data.harga.perMalam }} / malam
        </p>
        <p class="flex items-center font-bold mt-[5px] gap-x-1">
          <span class="text-xs leading-[14.06px] text-[#008489]">5.0</span>
          <svg
            width="8"
            height="8"
            viewBox="0 0 8 8"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M4 0L4.89806 2.76393H7.80423L5.45308 4.47214L6.35114 7.23607L4 5.52786L1.64886 7.23607L2.54692 4.47214L0.195774 2.76393H3.10194L4 0Z"
              fill="#008489"
            />
          </svg>
        </p>
      </div>
    </div>
  </section>
</template>

<script setup>
let dataTempat = [
  {
    id: 1,
    nama: "",
    wilayah: "Pulau Cayman",
    gambar: "_nuxt/assets/img/adventure1.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "petualangan",
  },
  {
    id: 2,
    nama: "",
    wilayah: "Uruguay",
    gambar: "_nuxt/assets/img/adventure2.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "petualangan",
  },
  {
    id: 3,
    nama: "",
    wilayah: "Islandia",
    gambar: "_nuxt/assets/img/adventure3.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "petualangan",
  },
  {
    id: 4,
    nama: "",
    wilayah: "Mongolia",
    gambar: "_nuxt/assets/img/adventure4.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "petualangan",
  },
  {
    id: 5,
    nama: "",
    wilayah: "Bahrain",
    gambar: "_nuxt/assets/img/adventure5.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "petualangan",
  },
  {
    id: 6,
    nama: "",
    wilayah: "Bosnia Dan Herzegovina",
    gambar: "_nuxt/assets/img/adventure6.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "petualangan",
  },
  {
    id: 7,
    nama: "",
    wilayah: "Toledo",
    gambar: "_nuxt/assets/img/housing1.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "perumahan",
  },
  {
    id: 8,
    nama: "",
    wilayah: "Mesa",
    gambar: "_nuxt/assets/img/housing2.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "perumahan",
  },
  {
    id: 9,
    nama: "",
    wilayah: "Utica",
    gambar: "_nuxt/assets/img/housing3.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "perumahan",
  },
  {
    id: 10,
    nama: "",
    wilayah: "South Bend",
    gambar: "_nuxt/assets/img/housing4.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "perumahan",
  },
  {
    id: 11,
    nama: "",
    wilayah: "Toledo",
    gambar: "_nuxt/assets/img/housing5.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "perumahan",
  },
  {
    id: 12,
    nama: "",
    wilayah: "Mesa",
    gambar: "_nuxt/assets/img/housing6.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "perumahan",
  },
  {
    id: 13,
    nama: "",
    wilayah: "Utica",
    gambar: "_nuxt/assets/img/housing7.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "perumahan",
  },
  {
    id: 14,
    nama: "",
    wilayah: "South Bend",
    gambar: "_nuxt/assets/img/housing8.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "perumahan",
  },
  {
    id: 15,
    nama: "",
    wilayah: "Pulau Cayman",
    gambar: "_nuxt/assets/img/experience1.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "pengalaman",
  },
  {
    id: 16,
    nama: "",
    wilayah: "Uruguay",
    gambar: "_nuxt/assets/img/experience2.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "pengalaman",
  },
  {
    id: 17,
    nama: "",
    wilayah: "Islandia",
    gambar: "_nuxt/assets/img/experience3.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "pengalaman",
  },
  {
    id: 18,
    nama: "",
    wilayah: "Mongolia",
    gambar: "_nuxt/assets/img/experience4.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "pengalaman",
  },
  {
    id: 19,
    nama: "",
    wilayah: "Bahrain",
    gambar: "_nuxt/assets/img/experience5.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "pengalaman",
  },
  {
    id: 20,
    nama: "",
    wilayah: "Bosnia Dan Herzegovina",
    gambar: "_nuxt/assets/img/experience6.png",
    deskripsi: "PAKET 2 Malam Semua Termasuk",
    harga: {
      perOrang: 100000,
      perMalam: 800000,
    },
    kategori: "pengalaman",
  },
];

dataTempat = dataTempat.filter((data) => data.kategori == "pengalaman");
</script>
