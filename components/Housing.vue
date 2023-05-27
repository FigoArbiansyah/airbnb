<template>
  <section class="md:px-[80px] px-5 pt-[88px]">
    <div>
      <h3 class="font-[700] leading-[28.13px] text-[24px] text-[#484848]">
        Logements dans le monde entier
      </h3>
    </div>
    <div class="mt-[51px] flex gap-x-4 gap-y-8 flex-wrap">
      <div v-for="data in dataTempat" class="md:w-[285px] w-full">
        <div class="w-full h-[200px] overflow-hidden rounded-[4px]">
          <img
            :src="data.gambar"
            class="w-full h-full object-cover hover:scale-110 transition-all ease duration-500 cursor-pointer"
            alt=""
          />
        </div>
        <div class="mt-2 flex justify-between">
          <div class="flex gap-x-[13px] items-center">
            <div
              class="border border-[#484848] p-2 font-bold text-[10px] leading-[11.72px] text-[#484848] uppercase"
            >
              <p>Superhost</p>
            </div>
            <p class="text-[#767676] text-xs leading-[14px] font-[400]">
              {{ data.wilayah }}
            </p>
          </div>
          <div
            class="flex gap-x-1 items-center font-[500] text-[12px] leading-[14px] text-[#484848]"
          >
            <svg
              width="8"
              height="8"
              viewBox="0 0 8 8"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M4 0L4.89806 2.76393H7.80423L5.45308 4.47214L6.35114 7.23607L4 5.52786L1.64886 7.23607L2.54692 4.47214L0.195774 2.76393H3.10194L4 0Z"
                fill="#FF5A5F"
              />
            </svg>

            <span>4,98</span>
          </div>
        </div>
        <p class="mt-2 text-[#484848] font-[14px] leading-[21px]">
          Dari Rp. {{ data.harga.perOrang }}/Orang - 3 Hari
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

dataTempat = dataTempat.filter((data) => data.kategori == "perumahan");
</script>
