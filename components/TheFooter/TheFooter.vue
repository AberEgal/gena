<template>
  <footer class="flex md:justify-between mx-4 pt-6 pb-4 mt-4 border-t border-teal-dark">
    <div>
      <ul class="flex list-reset">
        <li>
          <nuxt-link
            to="/impressum/"
            class="footer-link"
          >
            Impressum
          </nuxt-link>
        </li>
        <li>
          <nuxt-link
            to="/datenschutz/"
            class="footer-link"
          >
            Datenschutz
          </nuxt-link>
        </li>
        <li>
          <nuxt-link
            to="/richtlinien/"
            class="footer-link"
          >
            Richtlinien
          </nuxt-link>
        </li>
      </ul>
    </div>
    <div class="flex items-end text-xs text-teal-darker">
      &copy; 2019 by Generation Nachhaltigkeit
    </div>
  </footer>
</template>
