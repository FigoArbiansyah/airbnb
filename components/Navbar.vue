<template>
  <nav
    class="pl-[23px] pr-[24px] pt-[14px] flex justify-between items-end text-white fixed top-0 w-full z-50 transition-all ease"
  >
    <NuxtLink to="/">
      <img
        src="~/assets/img/logo.png"
        class="w-[30px] h-[32px] small-white-logo"
        alt=""
      />
      <svg
        class="small-red-logo hidden"
        width="30"
        height="32"
        viewBox="0 0 30 32"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M14.9762 24.0478C13.2422 21.8718 12.2222 19.9644 11.8822 18.3324C11.5422 17.0064 11.6782 15.9524 12.2562 15.1704C12.8682 14.2524 13.7862 13.8104 14.9762 13.8104C16.1662 13.8104 17.0842 14.2524 17.6962 15.1704C18.2742 15.9524 18.4102 17.0064 18.0702 18.3324C17.6962 19.9984 16.6762 21.9024 14.9762 24.0478ZM27.291 25.5098C27.053 27.1078 25.965 28.4338 24.469 29.0798C21.579 30.3378 18.7196 28.3318 16.2716 25.6118C20.321 20.5424 21.069 16.5984 19.3316 14.045C18.3116 12.583 16.8496 11.869 14.9762 11.869C11.2022 11.869 9.1248 15.065 9.9408 18.7744C10.4168 20.7804 11.6748 23.0618 13.6808 25.6118C12.4228 27.0058 11.2328 27.9918 10.1788 28.6038C9.3628 29.0458 8.5808 29.3178 7.8328 29.3858C4.3988 29.8958 1.70939 26.5638 2.93339 23.1264C3.10339 22.6844 3.4434 21.8684 4.02139 20.6104L4.0554 20.5424C5.9254 16.459 8.2068 11.835 10.8248 6.69755L10.8928 6.52755L11.6408 5.09955C12.2188 4.04555 12.4568 3.56955 13.3748 2.99155C13.8168 2.71955 14.3608 2.58355 14.9728 2.58355C16.1968 2.58355 17.1488 3.29755 17.5568 3.87555C17.7608 4.18155 17.9988 4.58955 18.3048 5.09955L19.0188 6.49355L19.1208 6.69755C21.7388 11.835 24.0202 16.459 25.8902 20.5424L25.9242 20.5764L26.6042 22.1404L27.0122 23.1264C27.325 23.9118 27.393 24.6938 27.291 25.5098ZM28.855 22.4464C28.617 21.6984 28.209 20.8144 27.699 19.7604V19.7264C25.285 14.589 23.0376 9.96495 20.8956 5.81355L20.7596 5.60955C19.2296 2.48155 18.1416 0.608154 14.9762 0.608154C11.8482 0.608154 10.5188 2.78415 9.1588 5.60955L9.0568 5.81355C6.9148 9.96495 4.66739 14.589 2.25339 19.7264V19.7944L1.53939 21.3584C1.26739 22.0044 1.13139 22.3444 1.09739 22.4464C-0.636605 27.2098 2.9334 31.3918 7.2548 31.3918C7.2888 31.3918 7.4248 31.3918 7.5948 31.3578H8.0708C10.3148 31.0858 12.6302 29.6578 14.9762 27.1044C17.3222 29.6544 19.6376 31.0858 21.8816 31.3578H22.3576C22.5276 31.3918 22.6636 31.3918 22.6976 31.3918C27.019 31.3952 30.589 27.2098 28.855 22.4464Z"
          fill="#FF5A5F"
        />
      </svg>
    </NuxtLink>
    <div class="max-md:top-0 max-md:left-0 max-md:absolute max-md:w-full">
      <ul
        class="nav-item flex gap-x-[25px] text-[14px] font-[500] max-md:flex-col max-md:absolute max-md:w-3/4 max-md:min-h-screen max-md:bg-white -right-[700px] max-md:text-black max-md:justify-center max-md:gap-y-10 max-md:pl-10 transition-all ease duration-500"
      >
        <!-- HAMBURGER MENU -->
        <li class="md:hidden right-10 top-10 flex flex-col">
          <span class="w-6 h-2 border-t-2 border-white top-burger"></span>
          <span class="w-6 h-2 border-t-2 border-white mid-burger"></span>
          <span class="w-6 h-2 border-t-2 border-white bot-burger"></span>
        </li>
        <!-- CLOSE BUTTON -->
        <li
          class="md:hidden absolute right-6 top-6 flex flex-col cursor-pointer"
          @click="closeNav()"
        >
          <span
            class="w-6 h-2 border-t-2 border-black rotate-45 mt-2 -ml-[2px]"
          ></span>
          <span
            class="w-6 h-2 border-t-2 border-black -rotate-45 -mt-2 ml-[2px]"
          ></span>
        </li>
        <li>
          <a href="#">Français (FR)</a>
        </li>
        <li>
          <a href="#">EUR €</a>
        </li>
        <li>
          <a href="#">Devenir hôte</a>
        </li>
        <li>
          <a href="#">Créer son expérience</a>
        </li>
        <li>
          <a href="#">Aide</a>
        </li>
        <li>
          <a href="#">Connexion</a>
        </li>
      </ul>
    </div>
    <div class="md:hidden cursor-pointer" @click="openNav()">
      <ul class="md:hidden">
        <li class="md:hidden right-10 top-10 flex flex-col">
          <span class="w-6 h-2 border-t-2 border-white"></span>
          <span class="w-6 h-2 border-t-2 border-white"></span>
          <span class="w-6 h-2 border-t-2 border-white"></span>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script setup>
const route = useRoute();
if (process.client) {
  const navScroll = () => {
    const nav = document.querySelector("nav");
    const topBurger = document.querySelector(".top-burger");
    const midBurger = document.querySelector(".mid-burger");
    const botBurger = document.querySelector(".bot-burger");
    if (route.name == "index") {
      if (
        document.documentElement.scrollTop > 50 ||
        document.body.scrollTop > 50
      ) {
        topBurger.classList.add("border-black");
        midBurger.classList.add("border-black");
        botBurger.classList.add("border-black");
        nav.classList.add("bg-white");
        nav.classList.remove("text-white");
        nav.classList.add("items-center");
        nav.classList.add("py-3");
        document.querySelector(".small-white-logo").classList.add("hidden");
        document.querySelector(".small-red-logo").classList.remove("hidden");
      } else {
        topBurger.classList.remove("border-black");
        midBurger.classList.remove("border-black");
        botBurger.classList.remove("border-black");
        nav.classList.remove("bg-white");
        nav.classList.add("text-white");
        nav.classList.remove("items-center");
        nav.classList.remove("py-3");
        document.querySelector(".small-white-logo").classList.remove("hidden");
        document.querySelector(".small-red-logo").classList.add("hidden");
      }
    } else {
      topBurger.classList.add("border-black");
      midBurger.classList.add("border-black");
      botBurger.classList.add("border-black");
      nav.classList.add("bg-white");
      nav.classList.add("text-black");
      nav.classList.add("items-center");
      nav.classList.add("py-3");
      document.querySelector(".small-white-logo").classList.add("hidden");
      document.querySelector(".small-red-logo").classList.remove("hidden");
    }
    window.addEventListener("scroll", navScroll);
  };
  navScroll();
}
const openNav = () => {
  const navItem = document.querySelector(".nav-item");
  navItem.classList.remove("-right-[700px]");
  navItem.classList.add("right-0");
};
const closeNav = () => {
  const navItem = document.querySelector(".nav-item");
  navItem.classList.add("-right-[700px]");
  navItem.classList.remove("right-0");
};
</script>
