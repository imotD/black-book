<template>
  <footer
    class="
      text-gray-700 text-sm
      leading-normal
      flex flex-wrap
      justify-between
      mx-auto
      max-w-3xl
      px-6
      sm:px-12
    "
  >
    <div class="w-full sm:w-1/2 mb-4 sm:mb-0">
      <p>
        The
        <a
          href="https://github.com/imotD/black-book"
          class="
            border-b border-transparent
            hover:border-gray-400
            transition-colors
            duration-300
          "
        >
          BlackBook
        </a>
        Template by
        <a
          href="https://gridsome-starter-bleda.netlify.app/"
          class="
            border-b border-transparent
            hover:border-gray-400
            transition-colors
            duration-300
          "
        >
          Bleda
        </a>
      </p>
      <p>Journal with feelings by <span class="text-red-900">imotD</span>.</p>
    </div>
    <div class="w-full sm:w-1/2">
      <nav>
        <ul class="flex sm:justify-end -mx-2">
          <li class="px-2">
            <g-link
              to="/"
              class="
                border-b border-transparent
                hover:border-gray-400
                transition-colors
                duration-300
              "
              >Home</g-link
            >
          </li>
          <li class="px-2">
            <g-link
              to="/about/"
              class="
                border-b border-transparent
                hover:border-gray-400
                transition-colors
                duration-300
              "
              >About</g-link
            >
          </li>
          <li class="px-2">
            <a
              href="https://saweria.co/dottomstyleart"
              class="
                border-b border-transparent
                hover:border-gray-400
                transition-colors
                duration-300
              "
              >Support</a
            >
          </li>
        </ul>
      </nav>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>
