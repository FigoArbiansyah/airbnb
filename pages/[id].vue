<template>
  <section class="pt-24 md:px-[88px] px-5">
    <div>
      <p class="text-[28px]">
        {{ dataTempat.wilayah }}
      </p>
      <div class="flex justify-between items-center">
        <div class="flex gap-x-[2px] items-center">
          <div class="flex items-center gap-[4px]">
            <svg
              width="16"
              height="16"
              viewBox="0 0 8 8"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M4 0L4.89806 2.76393H7.80423L5.45308 4.47214L6.35114 7.23607L4 5.52786L1.64886 7.23607L2.54692 4.47214L0.195774 2.76393H3.10194L4 0Z"
                fill="#484848"
              />
            </svg>
            <p class="text-sm">4.8</p>
          </div>
          <div>.</div>
          <div>
            <p class="text-sm underline">212 ulasan</p>
          </div>
          <div class="md:mx-1 mx-[2px]">.</div>
          <div class="flex md:gap-x-2 gap-x-1 items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 20 20"
              fill="currentColor"
              class="w-3 h-3"
            >
              <path
                fill-rule="evenodd"
                d="M10 1c-1.828 0-3.623.149-5.371.435a.75.75 0 00-.629.74v.387c-.827.157-1.642.345-2.445.564a.75.75 0 00-.552.698 5 5 0 004.503 5.152 6 6 0 002.946 1.822A6.451 6.451 0 017.768 13H7.5A1.5 1.5 0 006 14.5V17h-.75C4.56 17 4 17.56 4 18.25c0 .414.336.75.75.75h10.5a.75.75 0 00.75-.75c0-.69-.56-1.25-1.25-1.25H14v-2.5a1.5 1.5 0 00-1.5-1.5h-.268a6.453 6.453 0 01-.684-2.202 6 6 0 002.946-1.822 5 5 0 004.503-5.152.75.75 0 00-.552-.698A31.804 31.804 0 0016 2.562v-.387a.75.75 0 00-.629-.74A33.227 33.227 0 0010 1zM2.525 4.422C3.012 4.3 3.504 4.19 4 4.09V5c0 .74.134 1.448.38 2.103a3.503 3.503 0 01-1.855-2.68zm14.95 0a3.503 3.503 0 01-1.854 2.68C15.866 6.449 16 5.74 16 5v-.91c.496.099.988.21 1.475.332z"
                clip-rule="evenodd"
              />
            </svg>

            <span>HosTeladan</span>
          </div>
          <div class="md:mx-1 mx-[2px]">.</div>
          <div>
            <p class="text-sm underline">Abiansemal, Bali, Indonesia</p>
          </div>
        </div>
        <div class="max-md:hidden flex items-center gap-x-2.5">
          <div
            class="p-2 flex items-center gap-x-2 hover:bg-gray-100 rounded-lg transition-all ease cursor-pointer"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 20 20"
              fill="#333"
              class="w-4 h-4"
            >
              <path
                d="M9.25 13.25a.75.75 0 001.5 0V4.636l2.955 3.129a.75.75 0 001.09-1.03l-4.25-4.5a.75.75 0 00-1.09 0l-4.25 4.5a.75.75 0 101.09 1.03L9.25 4.636v8.614z"
              />
              <path
                d="M3.5 12.75a.75.75 0 00-1.5 0v2.5A2.75 2.75 0 004.75 18h10.5A2.75 2.75 0 0018 15.25v-2.5a.75.75 0 00-1.5 0v2.5c0 .69-.56 1.25-1.25 1.25H4.75c-.69 0-1.25-.56-1.25-1.25v-2.5z"
              />
            </svg>

            <p class="text-sm underline">Bagikan</p>
          </div>
          <div
            class="p-2 flex items-center gap-x-2 hover:bg-gray-100 rounded-lg transition-all ease cursor-pointer"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="#333"
              class="w-4 h-4"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M21 8.25c0-2.485-2.099-4.5-4.688-4.5-1.935 0-3.597 1.126-4.312 2.733-.715-1.607-2.377-2.733-4.313-2.733C5.1 3.75 3 5.765 3 8.25c0 7.22 9 12 9 12s9-4.78 9-12z"
              />
            </svg>

            <p class="text-sm underline">Simpan</p>
          </div>
        </div>
      </div>
    </div>
    <div
      class="mt-8 flex max-h-[20rem] w-full justify-between rounded-xl overflow-hidden items-center"
    >
      <div class="md:w-1/2 h-[20rem] overflow-hidden">
        <img
          :src="dataTempat.gambar"
          class="h-[20rem] w-full object-cover"
          alt=""
        />
      </div>
      <div
        class="max-md:hidden w-[49%] h-[20rem] flex flex-col justify-between gap-y-2.5"
      >
        <div class="flex gap-x-3">
          <img
            :src="dataTempat.gambar"
            class="h-[20rem] w-[49%] h-[10rem] object-cover"
            alt=""
          />
          <img
            :src="dataTempat.gambar"
            class="h-[20rem] w-[49%] h-[10rem] object-cover"
            alt=""
          />
        </div>
        <div class="flex gap-x-3">
          <img
            :src="dataTempat.gambar"
            class="h-[20rem] w-[49%] h-[10rem] object-cover"
            alt=""
          />
          <img
            :src="dataTempat.gambar"
            class="h-[20rem] w-[49%] h-[10rem] object-cover"
            alt=""
          />
        </div>
      </div>
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

const route = useRoute();

dataTempat = dataTempat.filter((data) => data.id == route.params.id)[0];
</script>
