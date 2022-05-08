<script>
export default {
  data() {
    return {
      message: "Hello world",
      emailme: "",
      errors: [],
    };
  },
  mounted() {
    console.log("Upload component", this.message);
  },
  methods: {
    collapse: function (e) {
      // set the target element that will be collapsed or expanded (eg. navbar menu)
      const targetEl = document.getElementById("targetEl");

      // optionally set a trigger element (eg. a button, hamburger icon)
      const triggerEl = document.getElementById("triggerEl");

      // optional options with default values and callback functions
      const options = {
        triggerEl: triggerEl,
        onCollapse: () => {
          console.log("element has been collapsed");
        },
        onExpand: () => {
          console.log("element has been expanded");
        },
        onToggle: () => {
          console.log("element has been toggled");
        },
      };
      console.log(this.$refs.targetEl);
      e.preventDefault();
    },
  },
};
</script>
<template>
  <div class="flex block md:hidden">
    <button
      id="triggerEl"
      class="w-7 navbar-toggler focus:outline-none"
      type="button"
      data-toggle="collapse"
      data-target="#mobile-menu"
      aria-controls="mobile-menu"
      aria-expanded="false"
      data-collapse-toggle="mobile-menu"
      aria-label="Toggle navigation"
    >
      <span class="toggler-icon bg-white"></span>
      <span class="toggler-icon"></span>
      <span class="toggler-icon"></span>
    </button>
    <a class="mr-4 navbar-brand block md:hidden" href="index.html">
      <img src="@/assets/logo.svg" alt="Logo" />
    </a>
  </div>
  <div
    class="relative left-0 z-3 hidden w-full px-5 py-3 duration-300 bg-[#2091F9] shadow md:opacity-100 md:w-auto collapse navbar-collapse md:block top-100 mt-full md:static md:bg-transparent md:shadow-none"
    id="mobile-menu"
  >
    <ul
      class="items-center content-start mr-auto lg:justify-center md:justify-end navbar-nav md:flex justify-self-end"
    >
      <li class="nav-item">
        <RouterLink to="/">Home</RouterLink>
      </li>
      <li class="nav-item">
        <RouterLink to="/product">Product</RouterLink>
      </li>
      <li class="nav-item">
        <RouterLink to="/princing">Pricing</RouterLink>
      </li>
      <li class="nav-item">
        <RouterLink to="/about">About</RouterLink>
      </li>
      <li class="nav-item">
        <RouterLink to="/about">Contact</RouterLink>
      </li>
    </ul>
  </div>
</template>

<style scoped></style>
