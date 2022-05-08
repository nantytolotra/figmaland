<script>
export default {
  name: "HomepageItem",
  data() {
    return {
      message: "Hello world",
      emailme: "Email me !",
    };
  },
  mounted() {
    console.log("Upload component", this.message);
  },
};
</script>
<template>
  <header>
    <div class="navigation">
      <div class="container">
        <div class="row">
          <div class="w-full">
            <nav
              class="grid md:flex items-center justify-items-stretch navbar navbar-expand-md"
            >
              <div class="items-center lg:w-36"></div>
              <slot name="navigation"></slot>
              <slot name="logo"></slot>
              <div class="items-center lg:w-80"></div>
              <div
                class="items-center justify-end hidden navbar-social lg:flex"
              >
                <slot name="social_network"></slot>
              </div>
              <slot></slot>
            </nav>
          </div>
        </div>
      </div>
    </div>
  </header>

  <slot name="header_content"></slot>
  <slot name="block_content_first">
    <section id="features" class="bg-gray-100 features-area py-120">
      <div class="container">
        <div class="justify-center row">
          <div class="w-full mx-4 lg:w-1/2">
            <div class="pb-10 text-center section-title">
              <h4 class="title">Features</h4>
              <p class="text">
                Most calendars are designed for teams.Slate is designed for
                freelancers
              </p>
            </div>
            <!-- section title -->
          </div>
        </div>
        <!-- row -->
      </div>
    </section>
  </slot>
  <slot name="block_video_first" :emailme="message"> </slot>
  <slot name="newsletter"> </slot>

  <slot name="partners"> </slot>
  <slot name="testimonial"> </slot>
  <slot name="pricing"> </slot>
  <slot name="contact"> </slot>
  <footer>
    <slot name="footer"> </slot>
  </footer>
</template>

<style scoped></style>
