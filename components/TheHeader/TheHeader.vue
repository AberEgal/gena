<template>
  <header class="flex justify-between items-center pt-6 pb-4 mb-4 border-b-4 border-teal-dark">
    <div>
      <nav class="hidden md:block">
        <nuxt-link
          to="/blog/"
          class="nav-link px-4"
        >
          Blog
        </nuxt-link>
        <nuxt-link
          to="/nachhaltigkeit/"
          class="nav-link px-4"
        >
          Nachhaltigkeit
        </nuxt-link>
        <nuxt-link
          to="/ueber-uns/"
          class="nav-link px-4"
        >
          Über uns
        </nuxt-link>
        <nuxt-link
          to="/kontakt/"
          class="nav-link px-4"
        >
          Kontakt
        </nuxt-link>
      </nav>
      <nav class="md:hidden">
        <img class="w-16 ml-4 mt-4" src="@/static/icons/burger-icon.svg" alt="Menu">
      </nav>
    </div>
    <div>
      <a
        href="https://www.facebook.com/"
        class="nav-link"
      >
        <img class="h-6 px-1" src="@/static/icons/icon-facebook.svg" alt="Facebook">
      </a>
      <a
        href="https://www.instagram.com/"
        class="nav-link"
      >
        <img class="h-6 px-1" src="@/static/icons/icon-instagram.svg" alt="Instagram">
      </a>
      <a
        href="https://www.twitter.com/"
        class="nav-link"
      >
        <img class="h-6 px-1" src="@/static/icons/icon-twitter.svg" alt="Twitter">
      </a>
    </div>
  </header>
</template>
