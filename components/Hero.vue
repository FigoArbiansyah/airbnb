<template>
  <section id="hero" class="h-[750px] w-full relative overflow-y-hidden">
    <ReservationCard />
    <div
      class="parallax h-[750p] w-full absolute top-0 left-0 right-0 bottom-0 bg-[url(~/assets/img/hero.png)]"
    ></div>
  </section>
</template>

<script>
if (process.client) {
  window.addEventListener("scroll", function () {
    var parallax = document.querySelector(".parallax");
    var scrolled = window.pageYOffset;
    parallax.style.transform = "translateY(" + scrolled * 0.5 + "px)";
  });
}
</script>
