<template>
  <nav
    class="top-0 fixed z-50 w-full flex flex-wrap items-center justify-between px-2 py-3 navbar-expand-lg bg-white shadow"
  >
    <div
      class="container px-4 mx-auto flex flex-wrap items-center justify-between"
    >
      <div
        class="w-full relative flex justify-between lg:w-auto lg:static lg:block lg:justify-start"
      >
        <router-link to="/">
          <a
            class="text-gray-800 text-sm font-bold leading-relaxed inline-block mr-4 py-2 whitespace-no-wrap uppercase"
            href="#pablo"
          >
            Link
          </a>
        </router-link>
      </div>
      <div
        class="lg:flex flex-grow items-center"
        :class="[navbarOpen ? 'block' : 'hidden']"
        id="example-navbar-warning"
      >
        <ul class="flex flex-col lg:flex-row list-none lg:ml-auto">
          <li class="flex items-center">
            <a
              class="hover:text-gray-600 text-gray-800 px-3 py-2 flex items-center text-xs font-bold"
              href="https://github.com/creativetimofficial/vue-notus?ref=vn-index-navbar"
            >
              <span class="inline-block ml-2">Buy Insurance</span>
            </a>
          </li>
          <li class="flex items-center">
            <a
              class="hover:text-gray-600 text-gray-800 px-3 py-2 flex items-center text-xs font-bold"
              href="https://github.com/creativetimofficial/vue-notus?ref=vn-index-navbar"
            >
              <span class="inline-block ml-2">Renew Insurance</span>
            </a>
          </li>
          <li class="flex items-center">
            <a
              class="hover:text-gray-600 text-gray-800 px-3 py-2 flex items-center text-xs font-bold"
              href="https://github.com/creativetimofficial/vue-notus?ref=vn-index-navbar"
            >
              <span class="inline-block ml-2">File a Claim</span>
            </a>
          </li>
          <li class="flex items-center">
            <a
              class="hover:text-gray-600 text-gray-800 px-3 py-2 flex items-center text-xs font-bold"
              href="https://github.com/creativetimofficial/vue-notus?ref=vn-index-navbar"
            >
              <span class="inline-block ml-2">Contact Us</span>
            </a>
          </li>
          <li class="flex items-center">
            <a
              class="hover:text-gray-600 text-gray-800 px-3 py-2 flex items-center text-xs font-bold"
              href="https://github.com/creativetimofficial/vue-notus?ref=vn-index-navbar"
            >
              <span class="inline-block ml-2">Faq</span>
            </a>
          </li>
          <li class="flex items-center">
            <button
              class="bg-green-500 text-white active:bg-green-600 text-xs font-bold px-4 py-2 rounded shadow hover:shadow-lg outline-none focus:outline-none lg:mr-1 lg:mb-0 ml-3 mb-3 ease-linear transition-all duration-150"
              type="button"
            >
              <i class="fas fa-user"></i> Sign in
            </button>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
// import IndexDropdown from "@/components/Dropdowns/IndexDropdown.vue";

export default {
  data() {
    return {
      navbarOpen: false,
    };
  },
  methods: {
    setNavbarOpen: function () {
      this.navbarOpen = !this.navbarOpen;
    },
  },
  components: {
    // IndexDropdown,
  },
};
</script>
