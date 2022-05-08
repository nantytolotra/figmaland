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
    checkForm: function (e) {
      this.errors = [];
      if (!this.emailme) {
        this.errors.push("Email Required ! ");
      } else if (!this.validEmail(this.email)) {
        this.errors.push("Valid email required. ");
      }
      e.preventDefault();
    },
    validEmail: function (email) {
      var re =
        /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
      re.test(email);
    },
  },
};
</script>
<template>
  <div class="grid grid-cols-3 gap-2">
    <div class="col-start-2 justify-self-center p-12">
      <h4
        class="text-[28px] font-normal p-8 leading-10 tracking-[0.2px] text-center"
      >
        Testimonials
      </h4>
    </div>
  </div>
  <div class="w-full">
    <div
      class="block mx-20 md:mx-40 services-content flex flex-col justify-items-center"
    >
      <div class="services-icon grid justify-items-center py-6 md:py-0">
        <img src="@/assets/logos_ibm.png" />
      </div>
      <div class="mb-8 ml-0 services-content media-body sm:ml-3">
        <p class="font-bold text-[13.5256px] md:text-[28px] text-center md:m-8">
          Most calendars are designed for teams. Slate is designed for
          freelancers who want a simple way to plan their schedule.
        </p>
      </div>
      <div class="services-icon grid justify-items-center">
        <div class="h-full flex flex-row">
          <img
            class="w-20 h-20 mx-auto rounded-full flex-initial"
            src="@/assets/profil.png"
            alt="user avatar"
            height="220"
            width="220"
            loading="lazy"
          />
          <div class="flex-initial w-48">
            <h6 class="text-lg font-semibold leading-none ml-5 py-4">
              Origin across
            </h6>
            <span class="text-[16px] text-gray-700 ml-5">Ui designer</span>
          </div>
        </div>
      </div>
    </div>
    <!-- services content -->
    <div class="flex justify-center p-6">
      <a
        class="mx-3 main-btn justify-self-center px-12 py-2"
        href="javascript:void(0)"
        >More Testimonials</a
      >
    </div>
  </div>
</template>

<style scoped></style>
