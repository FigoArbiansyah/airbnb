<template>
  <footer
    class="py-6 bg-[#484848] flex items-start md:px-20 px-5 max-md:flex-col max-md:gap-y-6 justify-between"
  >
    <div class="flex gap-x-2 items-center">
      <img src="~/assets/img/logo.png" alt="" />
      <p class="text-lg font-extrabold text-white">airbnb</p>
    </div>
    <div>
      <ul class="text-slate-200">
        <li>
          <NuxtLink to="/">Français (FR)</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/">EUR €</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/">Devenir hôte</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/">Créer son expérience</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/">Aide</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/">Connexion</NuxtLink>
        </li>
      </ul>
    </div>
  </footer>
</template>
