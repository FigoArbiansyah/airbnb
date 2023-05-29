<template>
  <section class="md:px-[80px] px-5 pt-[88px]">
    <div>
      <h3 class="font-[700] leading-[28.13px] text-[24px] text-[#484848]">
        Logements dans le monde entier
      </h3>
    </div>
    <div class="mt-[51px] flex gap-x-4 gap-y-8 flex-wrap">
      <NuxtLink
        v-for="data in dataTempat"
        class="md:w-[285px] w-full"
        :to="`/${data.id}`"
      >
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
      </NuxtLink>
    </div>
  </section>
</template>

<script setup>
import adventure1 from "~/assets/img/adventure1.png";
import adventure2 from "~/assets/img/adventure2.png";
import adventure3 from "~/assets/img/adventure3.png";
import adventure4 from "~/assets/img/adventure4.png";
import adventure5 from "~/assets/img/adventure5.png";
import adventure6 from "~/assets/img/adventure6.png";
import housing1 from "~/assets/img/housing1.png";
import housing2 from "~/assets/img/housing2.png";
import housing3 from "~/assets/img/housing3.png";
import housing4 from "~/assets/img/housing4.png";
import housing5 from "~/assets/img/housing5.png";
import housing6 from "~/assets/img/housing6.png";
import housing7 from "~/assets/img/housing7.png";
import housing8 from "~/assets/img/housing8.png";
import experience1 from "~/assets/img/experience1.png";
import experience2 from "~/assets/img/experience2.png";
import experience3 from "~/assets/img/experience3.png";
import experience4 from "~/assets/img/experience4.png";
import experience5 from "~/assets/img/experience5.png";
import experience6 from "~/assets/img/experience6.png";

let dataTempat = [
  {
    id: 1,
    nama: "",
    wilayah: "Pulau Cayman",
    gambar: adventure1,
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
    gambar: adventure2,
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
    gambar: adventure3,
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
    gambar: adventure4,
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
    gambar: adventure5,
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
    gambar: adventure6,
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
    gambar: housing1,
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
    gambar: housing2,
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
    gambar: housing3,
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
    gambar: housing4,
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
    gambar: housing5,
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
    gambar: housing6,
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
    gambar: housing7,
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
    gambar: housing8,
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
    gambar: experience1,
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
    gambar: experience2,
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
    gambar: experience3,
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
    gambar: experience4,
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
    gambar: experience5,
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
    gambar: experience6,
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
