<script setup lang="ts">
import HomepageItem from "./HomepageItem.vue";
import ContactItem from "./Contact.vue";
import Newsletter from "./Newsletter.vue";
import Testimonial from "./Testimonial.vue";
import Navigation from "./Navigation.vue";
import Footer from "./Footer.vue";
</script>

<template>
  <HomepageItem>
    <template #navigation>
      <Navigation />
    </template>
    <template #logo>
      <a class="mr-4 navbar-brand hidden md:block" href="index.html">
        <img src="@/assets/logo.svg" alt="Logo" />
      </a>
    </template>
    <template #social_network>
      <ul class="flex flex-row justify-self-center left-0 space-x-4">
        <li>
          <a href="#">
            <svg
              width="42"
              height="42"
              viewBox="0 0 42 42"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M37.6845 10.6854C36.4597 11.2137 35.1269 11.5939 33.754 11.742C35.1793 10.8952 36.2467 9.55742 36.7559 7.9796C35.4184 8.77527 33.9531 9.33321 32.4251 9.62867C31.7865 8.94593 31.0141 8.40203 30.156 8.03086C29.298 7.65969 28.3727 7.4692 27.4379 7.47127C23.6554 7.47127 20.6134 10.5373 20.6134 14.2997C20.6134 14.828 20.6775 15.3564 20.7815 15.8647C15.1179 15.5685 10.0666 12.8628 6.70842 8.72008C6.09652 9.76522 5.77587 10.9552 5.77981 12.1663C5.77981 14.5359 6.9846 16.6252 8.82179 17.854C7.7391 17.8114 6.68177 17.5138 5.73579 16.9854V17.0695C5.73579 20.3876 8.08131 23.1374 11.2073 23.7698C10.6204 23.9223 10.0166 24.0003 9.41017 24.002C8.96588 24.002 8.54561 23.958 8.12133 23.8979C8.98589 26.6037 11.5035 28.569 14.5015 28.633C12.156 30.4702 9.21805 31.5509 6.02798 31.5509C5.4556 31.5509 4.92726 31.5309 4.37891 31.4668C7.40487 33.4081 10.9952 34.5288 14.8617 34.5288C27.4139 34.5288 34.2823 24.1301 34.2823 15.1042C34.2823 14.808 34.2823 14.5118 34.2623 14.2156C35.5912 13.243 36.7559 12.0382 37.6845 10.6854Z"
                fill="white"
              />
            </svg>
          </a>
        </li>

        <li>
          <a href="#">
            <svg
              width="42"
              height="42"
              viewBox="0 0 42 42"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M35.7517 4.98962H6.29255C5.58409 4.98962 5.01172 5.562 5.01172 6.27046V35.7296C5.01172 36.438 5.58409 37.0104 6.29255 37.0104H35.7517C36.4601 37.0104 37.0325 36.438 37.0325 35.7296V6.27046C37.0325 5.562 36.4601 4.98962 35.7517 4.98962ZM32.0533 14.3357H29.4956C27.4903 14.3357 27.1021 15.2883 27.1021 16.6892V19.7752H31.8892L31.2648 24.6064H27.1021V37.0104H22.1108V24.6104H17.9361V19.7752H22.1108V16.2129C22.1108 12.0782 24.6365 9.82476 28.3268 9.82476C30.096 9.82476 31.613 9.95685 32.0573 10.0169V14.3357H32.0533Z"
                fill="white"
              />
            </svg>
          </a>
        </li>
        <li>
          <a href="#">
            <svg
              width="42"
              height="42"
              viewBox="0 0 42 42"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M35.736 4.98962H6.27692C5.56847 4.98962 4.99609 5.562 4.99609 6.27046V35.7296C4.99609 36.438 5.56847 37.0104 6.27692 37.0104H35.736C36.4445 37.0104 37.0169 36.438 37.0169 35.7296V6.27046C37.0169 5.562 36.4445 4.98962 35.736 4.98962ZM14.4943 32.2753H9.74317V16.9934H14.4943V32.2753ZM12.1207 14.9041C11.5761 14.9041 11.0437 14.7425 10.5908 14.44C10.1379 14.1374 9.78498 13.7073 9.57655 13.2041C9.36812 12.7009 9.31359 12.1472 9.41984 11.613C9.5261 11.0789 9.78837 10.5882 10.1735 10.203C10.5586 9.81792 11.0493 9.55565 11.5835 9.4494C12.1177 9.34314 12.6714 9.39768 13.1745 9.6061C13.6777 9.81453 14.1078 10.1675 14.4104 10.6203C14.713 11.0732 14.8745 11.6056 14.8745 12.1503C14.8705 13.6713 13.6377 14.9041 12.1207 14.9041ZM32.2818 32.2753H27.5347V24.8425C27.5347 23.0694 27.5027 20.7919 25.0651 20.7919C22.5955 20.7919 22.2153 22.7211 22.2153 24.7144V32.2753H17.4722V16.9934H22.0271V19.0828H22.0912C22.7236 17.882 24.2726 16.6132 26.5861 16.6132C31.3972 16.6132 32.2818 19.7792 32.2818 23.8939V32.2753Z"
                fill="white"
              />
            </svg>
          </a>
        </li>
      </ul>
    </template>
    <template #header_content>
      <div
        id="home"
        class="relative z-10 header-hero w-full h-full bg-indigo-200 bg-center bg-cover"
        style="background-image: url(./src/assets/background.jpg)"
      >
        <div class="container">
          <div class="justify-center row">
            <div class="w-full lg:w-1/3 xl:w-2/5">
              <div class="pt-64 pb-64 text-center header-content">
                <h3
                  class="mb-5 text-3xl font-semibold leading-tight text-[#fff] md:text-5xl"
                >
                  The best products start with Figma
                </h3>
                <p class="px-5 mb-10 text-xl text-[#fff]">
                  Most calendars are designed for teams.Slate is designed for
                  freelancers
                </p>
                <ul class="flex flex-wrap justify-center">
                  <li>
                    <a
                      class="mx-3 main-btn px-12 py-2"
                      href="javascript:void(0)"
                      >Try For Free</a
                    >
                  </li>
                </ul>
              </div>
              <!-- header content -->
            </div>
          </div>
          <!-- row -->
        </div>
        <!-- container -->
      </div>
      <!-- header content -->
    </template>
    <template #block_content_first>
      <div class="grid grid-cols-3 gap-2">
        <div class="col-start-2 justify-self-center p-12">
          <h4
            class="text-[28px] font-normal p-8 leading-10 tracking-[0.2px] text-center"
          >
            Features
          </h4>
          <p class="text text-center">
            Most calendars are designed for teams . Slate is designed for
            freelancers
          </p>
        </div>
      </div>
      <div class="flex justify-center">
        <!-- row start -->
        <div class="w-3/5 lg:w-3/3">
          <div class="row">
            <div class="w-full md:w-1/3">
              <div class="block mx-4 services-content flex flex-col">
                <div class="services-icon grid justify-items-center">
                  <svg
                    width="47"
                    height="47"
                    viewBox="0 0 47 47"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M14.6042 0.625C18.3117 0.625 21.8673 2.0978 24.4889 4.7194C27.1105 7.34101 28.5833 10.8967 28.5833 14.6042C28.5833 17.9846 27.3888 21.0854 25.3808 23.5H46.375V46.375H23.5V25.3808C21.0854 27.3888 17.9846 28.5833 14.6042 28.5833C10.8967 28.5833 7.34101 27.1105 4.7194 24.4889C2.0978 21.8673 0.625 18.3117 0.625 14.6042C0.625 10.8967 2.0978 7.34101 4.7194 4.7194C7.34101 2.0978 10.8967 0.625 14.6042 0.625Z"
                      fill="#2091F9"
                    />
                  </svg>
                </div>
                <div class="mb-8 ml-0 services-content media-body sm:ml-3">
                  <h4 class="services-title text-center">
                    OpenType features Variable fonts
                  </h4>
                  <p class="text text-center">
                    Slate helps you see how many more days you need to work to
                    reach your financial goal.
                  </p>
                </div>
              </div>
              <!-- services content -->
            </div>
            <div class="w-full md:w-1/3">
              <div class="block mx-4 services-content sm:flex flex flex-col">
                <div class="services-icon grid justify-items-center">
                  <svg
                    width="45"
                    height="42"
                    viewBox="0 0 45 42"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M18.2486 41.65C22.402 40.0167 21.492 35.5134 19.392 32.6667C17.3153 29.75 14.4453 27.7434 11.552 25.8067C9.48756 24.5055 7.64432 22.8829 6.09197 21C5.43863 20.23 4.10863 18.8067 5.46197 18.5267C6.83863 18.2467 9.21863 19.6 10.432 20.1134C12.5553 21 14.6553 22.0267 16.6153 23.24L18.972 19.2734C15.332 16.87 10.6653 14.7467 6.3253 14.1167C3.85197 13.7434 1.23863 14.2567 0.398634 16.94C-0.348033 19.25 0.841967 21.5834 2.1953 23.4034C5.39197 27.6734 10.362 29.7267 14.072 33.4134C14.8653 34.1834 15.822 35.0934 16.2886 36.1667C16.7786 37.1934 16.662 37.2634 15.5653 37.2634C12.672 37.2634 9.0553 35 6.69864 33.5067L4.34197 37.4734C7.91197 39.6667 13.8853 43.0967 18.2486 41.65ZM44.1253 5.25004C44.6386 4.7367 44.6386 3.8967 44.1253 3.4067L41.092 0.373369C40.8476 0.137831 40.5214 0.00622559 40.182 0.00622559C39.8425 0.00622559 39.5164 0.137831 39.272 0.373369L36.892 2.75337L41.7453 7.6067L44.1253 5.25004ZM21.1653 18.48V23.3334H26.0186L40.3686 8.98337L35.5153 4.13004L21.1653 18.48Z"
                      fill="#2091F9"
                    />
                  </svg>
                </div>
                <div class="mb-8 ml-0 services-content media-body sm:ml-3">
                  <h4 class="services-title text-center">
                    Design with real data
                  </h4>
                  <p class="text text-center">
                    Slate helps you see how many more days you need to work to
                    reach your financial goal.
                  </p>
                </div>
              </div>
              <!-- services content -->
            </div>
            <div class="w-full md:w-1/3">
              <div class="block mx-4 services-content sm:flex flex flex-col">
                <div class="services-icon grid justify-items-center">
                  <svg
                    width="49"
                    height="47"
                    viewBox="0 0 49 47"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M47.6366 4.76792L44.2308 1.36209C43.2904 0.37084 41.6383 0.37084 40.647 1.36209L17.8737 24.1354L24.8633 31.125L47.6366 8.35167C48.6279 7.36042 48.6279 5.70834 47.6366 4.76792ZM12.7904 28.5833C10.7681 28.5833 8.82864 29.3867 7.39868 30.8167C5.96871 32.2466 5.16536 34.1861 5.16536 36.2083C5.16536 39.5379 2.21703 41.2917 0.0820312 41.2917C2.42036 44.3925 6.4362 46.375 10.2487 46.375C12.9451 46.375 15.531 45.3039 17.4376 43.3973C19.3442 41.4906 20.4154 38.9047 20.4154 36.2083C20.4154 34.1861 19.612 32.2466 18.1821 30.8167C16.7521 29.3867 14.8126 28.5833 12.7904 28.5833Z"
                      fill="#2091F9"
                    />
                  </svg>
                </div>
                <div class="mb-8 ml-0 services-content media-body sm:ml-3">
                  <h4 class="services-title text-center">
                    Fastest way to take action
                  </h4>
                  <p class="text text-center">
                    Slate helps you see how many more days you need to work to
                    reach your financial goal.
                  </p>
                </div>
              </div>
              <!-- services content -->
            </div>
          </div>
          <!-- row -->
        </div>
        <!-- row -->
      </div>
      <!-- row end -->
    </template>
    <template #block_video_first>
      <div class="grid grid-cols-6 gap-4">
        <div class="col-start-2 col-span-4 ...">
          <img src="@/assets/video_screen.jpg" />
        </div>
      </div>
      <div
        class="sm:flex lg:grid grid-cols-2 gap-2 p-0 md:p-28 h-full place-items-center md:place-items-end"
      >
        <div
          class="w-full md:w-90 justify-self-center md:justify-self-end md:ml-8 sm:w-full md:px-20"
        >
          <div
            class="block mx-4 services-content grid justify-items-center md:justify-items-start md:-mt-4 md:px-8 md:py-2"
          >
            <h4
              class="text-[28px] text-center md:text-justify font-normal leading-10 tracking-[0.2px] mx-2 px-4 md:py-1"
            >
              Fatest way <br />
              to organize
            </h4>
            <p
              class="text mx-2 px-2.5 w-2/3 md:w-full text-center md:text-justify md:py-6"
            >
              Most calendars are designed for teams.
              <span class="hidden md:block">
                Slate is designed for freelancers</span
              >
            </p>
            <a
              class="mx-3 main-btn w-2/3 text-center px-12 py-2"
              href="javascript:void(0)"
              >Try For Free</a
            >
          </div>
        </div>
        <div
          class="w-full py-14 md:py-0 justify-items-center md:justify-items-start grid"
        >
          <img src="@/assets/macbook_pro.png" class="w-10/12 px-8" />
        </div>
      </div>

      <div class="lg:grid grid-cols-2 gap-2 p-0 h-full sm:flex md:p-14">
        <h3 class="text-[20px] text-center sm:hidden">At your fingertips</h3>
        <h2 class="text-[25px] text-center sm:hidden">Newsletter</h2>
        <h3 class="text-[20px] text-center sm:hidden">
          Most calendars are designed for teams. Slate is designed for
          freelancers
        </h3>

        <div
          class="w-9/12 justify-items-center grid p-2 md:p-0 px-14 md:justify-self-end"
        >
          <img src="@/assets/newsletter.png" />
        </div>
        <div class="w-full">
          <div class="block mx-4 services-content">
            <h3 class="text-[20px] hidden md:block">At your fingertips</h3>
            <h2 class="text-[48px] leading-10 hidden md:block">
              Lightning fast
              <span class="hidden md:block"
                ><br />
                prototyping</span
              >
            </h2>
          </div>
          <div class="block mx-4 services-content pt-6">
            <!--Newsletter -->
            <div
              class="w-full sm:w-full sm:max-w-full mx-auto justify-self-start"
            >
              <div class="p-6 sm:rounded-md">
                <Newsletter />
              </div>
            </div>

            <!--Newsletter -->
          </div>
        </div>
      </div>
    </template>
    <template #partners>
      <div class="grid md:grid-cols-3 gap-2">
        <div class="col-start-2 justify-self-center p-0 py-12 md:p-12">
          <h4
            class="text-[28px] font-normal p-2 md:p-8 leading-10 tracking-[0.2px] text-center"
          >
            Partners
          </h4>
          <p class="text text-center">
            Most calendars are designed for teams. Slate is designed for
            freelancers
          </p>
        </div>
      </div>
      <div
        class="mx-24 md:mx-64 my-2 md:my-0 sm:flex space-y-0 sm:flex-col md:grid md:grid-cols-4 md:p-0 justify-center"
      >
        <div
          class="block services-content flex flex-col py-6 md:py-0 border justify-items-center grid"
        >
          <div class="text-center">
            <h3>Client Name</h3>
          </div>
          <div class="mx-8">
            <img class="bg-cover" src="@/assets/logos_google.png" />
          </div>
        </div>
        <div
          class="block services-content flex flex-col py-6 md:py-0 border justify-items-center grid"
        >
          <div class="text-center">
            <h3>Client Name</h3>
          </div>
          <div class="mx-8">
            <img src="@/assets/amazon.png" />
          </div>
        </div>
        <div
          class="block services-content flex flex-col py-6 md:py-0 border justify-items-center grid"
        >
          <div class="text-center">
            <h3>Client Name</h3>
          </div>
          <div class="mx-8">
            <img src="@/assets/microsoft.png" />
          </div>
        </div>
        <div
          class="block border services-content flex flex-col py-6 md:py-0 hidden md:block justify-items-center"
        >
          <div class="text-center">
            <h3 class="text-center">Client Name</h3>
          </div>
          <div class="mx-8">
            <img src="@/assets/uber.png" />
          </div>
        </div>
      </div>
      <div
        class="mx-24 my-2 md:mx-64 md:my-0 space-y-0 sm:flex sm:flex-col md:grid md:grid-cols-4 justify-center md:p-0"
      >
        <div
          class="block services-content flex flex-col py-6 md:py-0 border hidden md:block justify-items-center"
        >
          <div class="text-center">
            <h3>Client Name</h3>
          </div>
          <div class="mx-8">
            <img class="bg-cover" src="@/assets/dropbox.png" />
          </div>
        </div>
        <div
          class="block services-content flex flex-col py-6 md:py-0 border hidden md:block justify-items-center"
        >
          <div class="text-center">
            <h3 class="text-center">Client Name</h3>
          </div>
          <div class="mx-8">
            <img src="@/assets/logos_google.png" />
          </div>
        </div>
        <div
          class="block services-content flex flex-col py-6 md:py-0 border hidden md:block justify-items-center"
        >
          <div class="text-center">
            <h3>Client Name</h3>
          </div>
          <div class="mx-8">
            <img src="@/assets/uber.png" />
          </div>
        </div>
        <div
          class="block services-content flex flex-col py-6 md:py-0 border hidden md:block justify-items-center"
        >
          <div class="text-center">
            <h3>Client Name</h3>
          </div>
          <div class="mx-8">
            <img src="@/assets/amazon.png" />
          </div>
        </div>
      </div>
      <div class="flex justify-center p-6">
        <a
          class="mx-3 main-btn justify-self-center px-12 py-2"
          href="javascript:void(0)"
          >Try For Free</a
        >
      </div>
    </template>
    <template #testimonial>
      <Testimonial />
    </template>
    <template #pricing>
      <div class="w-full bg-[#252B42] py-28 pt-8">
        <div class="grid grid-cols-3 gap-2 py-6">
          <div class="col-start-2 justify-self-center p-0 mt-8">
            <h4
              class="text-[28px] text-[#fff] font-normal p-0 leading-10 tracking-[0.2px] text-center"
            >
              Pricing
            </h4>
            <p class="text text-center text-[#fff]">
              Most calendars are designed for teams.
              <span class="hidden md:block">
                Slate is designed for freelancers</span
              >
            </p>
          </div>
        </div>
        <div
          class="flex flex-col sm:flex-row justify-center mb-6 sm:mb-0 m-8 md:space-x-4"
        >
          <div
            class="flex-1 lg:flex-initial lg:w-1/4 rounded-lg bg-white mt-4 flex flex-col"
          >
            <div class="p-8 text-3xl font-bold text-center">
              <h3 class="text-[20px] leading-5">Free</h3>
              <h6 class="text-[16px] font-normal text-center">
                Organize across all apps by hand
              </h6>
            </div>
            <div class="border-0 border-grey-light text-sm">
              <div
                class="text-center border-0 border-grey-light py-4 flex flex-row justify-center"
              >
                <h1 class="text-[74px]">0</h1>
                <div>
                  <h3 class="text-[20px]">$</h3>
                  <h3 class="text-[16px]">Per Month</h3>
                </div>
              </div>
              <div class="text-center border-0 border-grey-light py-4">
                Pricing Feature
              </div>
              <div class="text-center border-0 border-grey-light py-4">
                Pricing Feature
              </div>
              <div class="text-center border-0 border-grey-light py-4">
                Pricing Feature
              </div>
              <div class="text-center border-0 border-grey-light py-4">
                Pricing Feature
              </div>
              <div class="text-center border-0 border-grey-light py-4">
                Pricing Feature
              </div>
            </div>
            <div class="text-center mt-8 mb-8 mt-auto">
              <a
                href="#"
                class="inline-block mx-3 main-btn text-white px-6 py-4 hover:bg-green-darker hover:text-white hover:no-underline"
                >Order Now</a
              >
            </div>
          </div>
          <div
            class="flex-1 lg:flex-initial lg:w-1/4 rounded-lg mt-4 sm:-mb-10 sm:-mt-8 shadow z-30 flex flex-col py-2 bg-[#2091F9]"
          >
            <div class="w-full p-8 text-3xl font-bold text-center">
              <h3 class="text-white">Standard</h3>
              <h6 class="text-[16px] font-normal text-center text-white">
                Organize across all apps by hand
              </h6>
            </div>

            <div class="w-full border-0 border-grey-light text-sm">
              <div
                class="text-center border-0 border-grey-light py-4 flex flex-row justify-center"
              >
                <h1 class="text-[74px] text-white">10</h1>
                <div>
                  <h3 class="text-[20px] text-white">$</h3>
                  <h3 class="text-[16px] text-white">Per Month</h3>
                </div>
              </div>
              <div
                class="text-center border-0 border-grey-light py-4 text-white"
              >
                Pricing Feature
              </div>
              <div
                class="text-center border-0 border-grey-light py-4 text-white"
              >
                Pricing Feature
              </div>
              <div
                class="text-center border-0 border-grey-light py-4 text-white"
              >
                Pricing Feature
              </div>
              <div
                class="text-center border-0 border-grey-light py-4 text-white"
              >
                Pricing Feature
              </div>
              <div
                class="text-center border-0 border-grey-light py-4 text-white"
              >
                Pricing Feature
              </div>
            </div>

            <div class="w-full text-center mb-8 mt-auto">
              <a
                href="#"
                class="inline-block mx-3 main-btn1 text-white px-6 py-4 rounded hover:bg-green-darker hover:text-white hover:no-underline"
                >Order Now</a
              >
            </div>
          </div>
          <div
            class="flex-1 lg:flex-initial lg:w-1/4 rounded-lg bg-white mt-4 flex flex-col"
          >
            <div class="p-8 text-3xl font-bold text-center">
              <h3 class="text-[20px] leading-5">BUSINESS</h3>
              <h6 class="text-[16px] font-normal text-center">
                Organize across all apps by hand
              </h6>
            </div>
            <div class="border-0 border-grey-light text-sm">
              <div
                class="text-center border-0 border-grey-light py-4 flex flex-row justify-center"
              >
                <h1 class="text-[74px]">99</h1>
                <div>
                  <h3 class="text-[20px]">$</h3>
                  <h3 class="text-[16px]">Per Month</h3>
                </div>
              </div>
              <div class="text-center border-0 border-grey-light py-4">
                Pricing Feature
              </div>
              <div class="text-center border-0 border-grey-light py-4">
                Pricing Feature
              </div>
              <div class="text-center border-0 border-grey-light py-4">
                Pricing Feature
              </div>
              <div class="text-center border-0 border-grey-light py-4">
                Pricing Feature
              </div>
              <div class="text-center border-0 border-grey-light py-4">
                Pricing Feature
              </div>
            </div>

            <div class="text-center pt-8 mb-8 mt-auto">
              <a
                href="#"
                class="inline-block mx-3 main-btn text-white px-6 py-4 mx-3 main-btn hover:bg-green-darker hover:text-white hover:no-underline"
                >Order Now</a
              >
            </div>
          </div>
        </div>
      </div>
    </template>
    <template #contact>
      <div class="grid grid-cols-3 gap-2">
        <div class="col-start-2 justify-self-center p-0 mt-10">
          <h4
            class="text-[28px] font-normal p-8 leading-10 tracking-[0.2px] text-center"
          >
            Contact Us
          </h4>
          <p class="text text-center">
            Most calendars are designed for teams.
            <span class="hidden md:block"
              >Slate is designed for freelancers</span
            >
          </p>
        </div>
      </div>
      <div class="flex space-x-4 py-12 justify-center md:hidden">
        <svg
          width="34"
          height="28"
          viewBox="0 0 34 28"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M33.6455 4.0808C32.4207 4.60914 31.0878 4.98939 29.7149 5.13749C31.1403 4.29068 32.2077 2.95287 32.7168 1.37505C31.3793 2.17072 29.914 2.72866 28.386 3.02412C27.7474 2.34138 26.975 1.79748 26.117 1.42631C25.2589 1.05514 24.3337 0.864651 23.3988 0.866716C19.6163 0.866716 16.5744 3.93271 16.5744 7.69515C16.5744 8.22349 16.6384 8.75183 16.7425 9.26016C11.0788 8.96397 6.02753 6.25821 2.66936 2.11553C2.05746 3.16067 1.7368 4.35068 1.74075 5.56176C1.74075 7.9313 2.94553 10.0207 4.78273 11.2495C3.70004 11.2068 2.64271 10.9092 1.69672 10.3809V10.4649C1.69672 13.7831 4.04225 16.5329 7.16827 17.1653C6.58133 17.3178 5.97753 17.3957 5.37111 17.3974C4.92682 17.3974 4.50655 17.3534 4.08227 17.2934C4.94683 19.9991 7.46447 21.9644 10.4624 22.0284C8.11689 23.8656 5.17898 24.9463 1.98891 24.9463C1.41654 24.9463 0.8882 24.9263 0.339844 24.8623C3.36581 26.8035 6.95614 27.9243 10.8226 27.9243C23.3748 27.9243 30.2432 17.5255 30.2432 8.49967C30.2432 8.20348 30.2432 7.90728 30.2232 7.61109C31.5521 6.63846 32.7168 5.43368 33.6455 4.0808Z"
            fill="#2091F9"
          />
        </svg>
        <svg
          width="33"
          height="33"
          viewBox="0 0 33 33"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M31.7126 0.385254H2.25349C1.54503 0.385254 0.972656 0.957625 0.972656 1.66609V31.1252C0.972656 31.8337 1.54503 32.406 2.25349 32.406H31.7126C32.4211 32.406 32.9934 31.8337 32.9934 31.1252V1.66609C32.9934 0.957625 32.4211 0.385254 31.7126 0.385254ZM28.0142 9.73132H25.4565C23.4512 9.73132 23.063 10.6839 23.063 12.0848V15.1708H27.8501L27.2257 20.002H23.063V32.406H18.0718V20.006H13.897V15.1708H18.0718V11.6085C18.0718 7.47385 20.5974 5.22039 24.2878 5.22039C26.0569 5.22039 27.5739 5.35248 28.0182 5.41252V9.73132H28.0142Z"
            fill="#2091F9"
          />
        </svg>
        <svg
          width="33"
          height="33"
          viewBox="0 0 33 33"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M31.697 0.385254H2.23786C1.5294 0.385254 0.957031 0.957625 0.957031 1.66609V31.1252C0.957031 31.8337 1.5294 32.406 2.23786 32.406H31.697C32.4054 32.406 32.9778 31.8337 32.9778 31.1252V1.66609C32.9778 0.957625 32.4054 0.385254 31.697 0.385254ZM10.4552 27.671H5.70411V12.389H10.4552V27.671ZM8.08165 10.2997C7.53701 10.2997 7.00459 10.1382 6.55173 9.83559C6.09887 9.533 5.74591 9.10292 5.53749 8.59973C5.32906 8.09654 5.27453 7.54285 5.38078 7.00866C5.48704 6.47448 5.74931 5.9838 6.13443 5.59868C6.51956 5.21355 7.01023 4.95128 7.54442 4.84503C8.0786 4.73877 8.63229 4.7933 9.13548 5.00173C9.63867 5.21016 10.0688 5.56312 10.3713 6.01598C10.6739 6.46884 10.8354 7.00125 10.8354 7.5459C10.8314 9.06689 9.59864 10.2997 8.08165 10.2997ZM28.2427 27.671H23.4957V20.2381C23.4957 18.465 23.4636 16.1875 21.0261 16.1875C18.5565 16.1875 18.1762 18.1168 18.1762 20.1101V27.671H13.4331V12.389H17.9881V14.4784H18.0521C18.6845 13.2776 20.2335 12.0088 22.547 12.0088C27.3582 12.0088 28.2427 15.1748 28.2427 19.2895V27.671Z"
            fill="#2091F9"
          />
        </svg>
      </div>
      <div class="flex justify-start block md:hidden">
        <!-- row start -->

        <div class="w-full lg:w-3/3">
          <div class="row">
            <div class="w-full md:w-1/3">
              <div class="block mx-4 services-content flex flex-col-2">
                <div class="services-icon">
                  <svg
                    width="28"
                    height="23"
                    viewBox="0 0 28 23"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <g clip-path="url(#clip0_67_7936)">
                      <path
                        d="M25.8125 0.904785H1.4375C0.918945 0.904785 0.5 1.32373 0.5 1.84229V20.5923C0.5 21.1108 0.918945 21.5298 1.4375 21.5298H25.8125C26.3311 21.5298 26.75 21.1108 26.75 20.5923V1.84229C26.75 1.32373 26.3311 0.904785 25.8125 0.904785ZM24.6406 4.15088V19.4204H2.60938V4.15088L1.80078 3.521L2.95215 2.0415L4.20605 3.01709H23.0469L24.3008 2.0415L25.4521 3.521L24.6406 4.15088ZM23.0469 3.01416L13.625 10.3384L4.20312 3.01416L2.94922 2.03857L1.79785 3.51807L2.60645 4.14795L12.6143 11.9292C12.9021 12.1528 13.2561 12.2742 13.6206 12.2742C13.9851 12.2742 14.3391 12.1528 14.627 11.9292L24.6406 4.15088L25.4492 3.521L24.2979 2.0415L23.0469 3.01416Z"
                        fill="#2091F9"
                      />
                    </g>
                    <defs>
                      <clipPath id="clip0_67_7936">
                        <rect
                          width="27"
                          height="22"
                          fill="white"
                          transform="translate(0.5 0.217285)"
                        />
                      </clipPath>
                    </defs>
                  </svg>
                </div>
                <div class="mb-8 ml-0 services-content media-body sm:ml-3">
                  <h6 class="text-center text-sm text-[16px] sm:ml-3">
                    6386 Spring St undefined Anchorage, Georgia 12473 United
                    States
                  </h6>
                </div>
              </div>
              <!-- services content -->
            </div>
            <div class="w-full md:w-1/3">
              <div class="block mx-4 services-content sm:flex flex flex-col-2">
                <div class="services-icon grid">
                  <svg
                    width="22"
                    height="35"
                    viewBox="0 0 22 35"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <g clip-path="url(#clip0_67_7930)">
                      <path
                        d="M16.5417 1.17578H4.875C2.45417 1.17578 0.5 3.12995 0.5 5.55078V28.8841C0.5 31.3049 2.45417 33.2591 4.875 33.2591H16.5417C18.9625 33.2591 20.9167 31.3049 20.9167 28.8841V5.55078C20.9167 3.12995 18.9625 1.17578 16.5417 1.17578ZM13.625 30.3424H7.79167V28.8841H13.625V30.3424ZM18.3646 25.9674H3.05208V5.55078H18.3646V25.9674Z"
                        fill="#2091F9"
                      />
                    </g>
                    <defs>
                      <clipPath id="clip0_67_7930">
                        <rect
                          width="21"
                          height="34"
                          fill="white"
                          transform="translate(0.5 0.217285)"
                        />
                      </clipPath>
                    </defs>
                  </svg>
                </div>
                <div class="mb-8 services-content media-body sm:ml-3">
                  <h6 class="text-center text-sm text-[16px] ml-12 sm:ml-8">
                    willie.jennings@example.com
                  </h6>
                </div>
              </div>
              <!-- services content -->
            </div>
            <div class="w-full md:w-1/3">
              <div class="block mx-4 services-content sm:flex flex flex-col-2">
                <div class="services-icon grid justify-items-center">
                  <svg
                    width="26"
                    height="33"
                    viewBox="0 0 26 33"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <g clip-path="url(#clip0_67_7924)">
                      <path
                        d="M13.0013 19.884C16.4941 19.884 19.3346 17.0435 19.3346 13.5506C19.3346 10.0578 16.4941 7.21729 13.0013 7.21729C9.50847 7.21729 6.66797 10.0578 6.66797 13.5506C6.66797 17.0435 9.50847 19.884 13.0013 19.884ZM13.0013 10.384C14.7477 10.384 16.168 11.8042 16.168 13.5506C16.168 15.297 14.7477 16.7173 13.0013 16.7173C11.2549 16.7173 9.83464 15.297 9.83464 13.5506C9.83464 11.8042 11.2549 10.384 13.0013 10.384Z"
                        fill="#2091F9"
                      />
                      <path
                        d="M11.7485 32.256C12.0164 32.4473 12.3375 32.5502 12.6668 32.5502C12.9961 32.5502 13.3172 32.4473 13.5851 32.256C14.0665 31.9155 25.3794 23.7471 25.3335 13.5505C25.3335 6.56637 19.6509 0.883789 12.6668 0.883789C5.68272 0.883789 0.000139393 6.56637 0.000139393 13.5425C-0.0457773 23.7471 11.2671 31.9155 11.7485 32.256ZM12.6668 4.05046C17.9061 4.05046 22.1668 8.31121 22.1668 13.5584C22.2001 20.5852 15.2191 26.8948 12.6668 28.9642C10.1161 26.8932 3.13356 20.582 3.16681 13.5505C3.16681 8.31121 7.42756 4.05046 12.6668 4.05046Z"
                        fill="#2091F9"
                      />
                    </g>
                    <defs>
                      <clipPath id="clip0_67_7924">
                        <rect
                          width="26"
                          height="32"
                          fill="white"
                          transform="translate(0 0.717285)"
                        />
                      </clipPath>
                    </defs>
                  </svg>
                </div>
                <div class="mb-8 ml-0 services-content media-body sm:ml-3">
                  <h6 class="text-center text-sm ml-12 sm:ml-8">
                    (843) 555-0130
                  </h6>
                </div>
              </div>
              <!-- services content -->
            </div>
          </div>
          <!-- row -->
        </div>
        <!-- row -->
      </div>

      <div class="lg:grid grid-cols-3 gap-2 p-0 h-full sm:flex md:p-28">
        <div
          class="shadow-lg border-solid border-2 services-content border-black-600 rounded-md flex flex-col mx-4 justify-items-center"
        >
          <ContactItem />
        </div>
        	
        <div class="flex flex-col mx-4 hidden md:block col-start-2 col-span-2">
          <div class="flex justify-start">
            <!-- row start -->
            <div class="w-full lg:w-3/3">
              <div class="row">
                <div class="w-full md:w-1/3">
                  <div class="block mx-4 services-content flex flex-col">
                    <div class="services-icon grid justify-items-center">
                      <svg
                        width="28"
                        height="23"
                        viewBox="0 0 28 23"
                        fill="none"
                        xmlns="http://www.w3.org/2000/svg"
                      >
                        <g clip-path="url(#clip0_67_7936)">
                          <path
                            d="M25.8125 0.904785H1.4375C0.918945 0.904785 0.5 1.32373 0.5 1.84229V20.5923C0.5 21.1108 0.918945 21.5298 1.4375 21.5298H25.8125C26.3311 21.5298 26.75 21.1108 26.75 20.5923V1.84229C26.75 1.32373 26.3311 0.904785 25.8125 0.904785ZM24.6406 4.15088V19.4204H2.60938V4.15088L1.80078 3.521L2.95215 2.0415L4.20605 3.01709H23.0469L24.3008 2.0415L25.4521 3.521L24.6406 4.15088ZM23.0469 3.01416L13.625 10.3384L4.20312 3.01416L2.94922 2.03857L1.79785 3.51807L2.60645 4.14795L12.6143 11.9292C12.9021 12.1528 13.2561 12.2742 13.6206 12.2742C13.9851 12.2742 14.3391 12.1528 14.627 11.9292L24.6406 4.15088L25.4492 3.521L24.2979 2.0415L23.0469 3.01416Z"
                            fill="#2091F9"
                          />
                        </g>
                        <defs>
                          <clipPath id="clip0_67_7936">
                            <rect
                              width="27"
                              height="22"
                              fill="white"
                              transform="translate(0.5 0.217285)"
                            />
                          </clipPath>
                        </defs>
                      </svg>
                    </div>
                    <div class="mb-8 ml-0 services-content media-body sm:ml-3">
                      <h6 class="text-center text-sm">
                        6386 Spring St undefined Anchorage, Georgia 12473 United
                        States
                      </h6>
                    </div>
                  </div>
                  <!-- services content -->
                </div>
                <div class="w-full md:w-1/3">
                  <div
                    class="block mx-4 services-content sm:flex flex flex-col"
                  >
                    <div class="services-icon grid justify-items-center">
                      <svg
                        width="22"
                        height="35"
                        viewBox="0 0 22 35"
                        fill="none"
                        xmlns="http://www.w3.org/2000/svg"
                      >
                        <g clip-path="url(#clip0_67_7930)">
                          <path
                            d="M16.5417 1.17578H4.875C2.45417 1.17578 0.5 3.12995 0.5 5.55078V28.8841C0.5 31.3049 2.45417 33.2591 4.875 33.2591H16.5417C18.9625 33.2591 20.9167 31.3049 20.9167 28.8841V5.55078C20.9167 3.12995 18.9625 1.17578 16.5417 1.17578ZM13.625 30.3424H7.79167V28.8841H13.625V30.3424ZM18.3646 25.9674H3.05208V5.55078H18.3646V25.9674Z"
                            fill="#2091F9"
                          />
                        </g>
                        <defs>
                          <clipPath id="clip0_67_7930">
                            <rect
                              width="21"
                              height="34"
                              fill="white"
                              transform="translate(0.5 0.217285)"
                            />
                          </clipPath>
                        </defs>
                      </svg>
                    </div>
                    <div class="mb-8 ml-0 services-content media-body sm:ml-3">
                      <h6 class="text-center text-sm">
                        willie.jennings@example.com
                      </h6>
                    </div>
                  </div>
                  <!-- services content -->
                </div>
                <div class="w-full md:w-1/3">
                  <div
                    class="block mx-4 services-content sm:flex flex flex-col"
                  >
                    <div class="services-icon grid justify-items-center">
                      <svg
                        width="26"
                        height="33"
                        viewBox="0 0 26 33"
                        fill="none"
                        xmlns="http://www.w3.org/2000/svg"
                      >
                        <g clip-path="url(#clip0_67_7924)">
                          <path
                            d="M13.0013 19.884C16.4941 19.884 19.3346 17.0435 19.3346 13.5506C19.3346 10.0578 16.4941 7.21729 13.0013 7.21729C9.50847 7.21729 6.66797 10.0578 6.66797 13.5506C6.66797 17.0435 9.50847 19.884 13.0013 19.884ZM13.0013 10.384C14.7477 10.384 16.168 11.8042 16.168 13.5506C16.168 15.297 14.7477 16.7173 13.0013 16.7173C11.2549 16.7173 9.83464 15.297 9.83464 13.5506C9.83464 11.8042 11.2549 10.384 13.0013 10.384Z"
                            fill="#2091F9"
                          />
                          <path
                            d="M11.7485 32.256C12.0164 32.4473 12.3375 32.5502 12.6668 32.5502C12.9961 32.5502 13.3172 32.4473 13.5851 32.256C14.0665 31.9155 25.3794 23.7471 25.3335 13.5505C25.3335 6.56637 19.6509 0.883789 12.6668 0.883789C5.68272 0.883789 0.000139393 6.56637 0.000139393 13.5425C-0.0457773 23.7471 11.2671 31.9155 11.7485 32.256ZM12.6668 4.05046C17.9061 4.05046 22.1668 8.31121 22.1668 13.5584C22.2001 20.5852 15.2191 26.8948 12.6668 28.9642C10.1161 26.8932 3.13356 20.582 3.16681 13.5505C3.16681 8.31121 7.42756 4.05046 12.6668 4.05046Z"
                            fill="#2091F9"
                          />
                        </g>
                        <defs>
                          <clipPath id="clip0_67_7924">
                            <rect
                              width="26"
                              height="32"
                              fill="white"
                              transform="translate(0 0.717285)"
                            />
                          </clipPath>
                        </defs>
                      </svg>
                    </div>
                    <div class="mb-8 ml-0 services-content media-body sm:ml-3">
                      <h6 class="text-center text-sm">(843) 555-0130</h6>
                    </div>
                  </div>
                  <!-- services content -->
                </div>
              </div>
              <!-- row -->
            </div>
            <!-- row -->
          </div>

          <div class="w-full h-1/2 flex hidden md:block">
            <iframe
              class="justify-items-center"
              width="100%"
              height="90%"
              frameborder="0"
              scrolling="no"
              marginheight="0"
              marginwidth="0"
              src="https://maps.google.com/maps?width=100%25&amp;height=600&amp;hl=en&amp;q=6386%20Spring%20United%20states+(My%20Business%20Name)&amp;t=&amp;z=14&amp;ie=UTF8&amp;iwloc=B&amp;output=embed"
              ><a href="https://www.gps.ie/marine-gps/">ship tracker</a></iframe
            >
          </div>
          <div class="flex space-x-4 py-12">
            <svg
              width="34"
              height="28"
              viewBox="0 0 34 28"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M33.6455 4.0808C32.4207 4.60914 31.0878 4.98939 29.7149 5.13749C31.1403 4.29068 32.2077 2.95287 32.7168 1.37505C31.3793 2.17072 29.914 2.72866 28.386 3.02412C27.7474 2.34138 26.975 1.79748 26.117 1.42631C25.2589 1.05514 24.3337 0.864651 23.3988 0.866716C19.6163 0.866716 16.5744 3.93271 16.5744 7.69515C16.5744 8.22349 16.6384 8.75183 16.7425 9.26016C11.0788 8.96397 6.02753 6.25821 2.66936 2.11553C2.05746 3.16067 1.7368 4.35068 1.74075 5.56176C1.74075 7.9313 2.94553 10.0207 4.78273 11.2495C3.70004 11.2068 2.64271 10.9092 1.69672 10.3809V10.4649C1.69672 13.7831 4.04225 16.5329 7.16827 17.1653C6.58133 17.3178 5.97753 17.3957 5.37111 17.3974C4.92682 17.3974 4.50655 17.3534 4.08227 17.2934C4.94683 19.9991 7.46447 21.9644 10.4624 22.0284C8.11689 23.8656 5.17898 24.9463 1.98891 24.9463C1.41654 24.9463 0.8882 24.9263 0.339844 24.8623C3.36581 26.8035 6.95614 27.9243 10.8226 27.9243C23.3748 27.9243 30.2432 17.5255 30.2432 8.49967C30.2432 8.20348 30.2432 7.90728 30.2232 7.61109C31.5521 6.63846 32.7168 5.43368 33.6455 4.0808Z"
                fill="#2091F9"
              />
            </svg>
            <svg
              width="33"
              height="33"
              viewBox="0 0 33 33"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M31.7126 0.385254H2.25349C1.54503 0.385254 0.972656 0.957625 0.972656 1.66609V31.1252C0.972656 31.8337 1.54503 32.406 2.25349 32.406H31.7126C32.4211 32.406 32.9934 31.8337 32.9934 31.1252V1.66609C32.9934 0.957625 32.4211 0.385254 31.7126 0.385254ZM28.0142 9.73132H25.4565C23.4512 9.73132 23.063 10.6839 23.063 12.0848V15.1708H27.8501L27.2257 20.002H23.063V32.406H18.0718V20.006H13.897V15.1708H18.0718V11.6085C18.0718 7.47385 20.5974 5.22039 24.2878 5.22039C26.0569 5.22039 27.5739 5.35248 28.0182 5.41252V9.73132H28.0142Z"
                fill="#2091F9"
              />
            </svg>
            <svg
              width="33"
              height="33"
              viewBox="0 0 33 33"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M31.697 0.385254H2.23786C1.5294 0.385254 0.957031 0.957625 0.957031 1.66609V31.1252C0.957031 31.8337 1.5294 32.406 2.23786 32.406H31.697C32.4054 32.406 32.9778 31.8337 32.9778 31.1252V1.66609C32.9778 0.957625 32.4054 0.385254 31.697 0.385254ZM10.4552 27.671H5.70411V12.389H10.4552V27.671ZM8.08165 10.2997C7.53701 10.2997 7.00459 10.1382 6.55173 9.83559C6.09887 9.533 5.74591 9.10292 5.53749 8.59973C5.32906 8.09654 5.27453 7.54285 5.38078 7.00866C5.48704 6.47448 5.74931 5.9838 6.13443 5.59868C6.51956 5.21355 7.01023 4.95128 7.54442 4.84503C8.0786 4.73877 8.63229 4.7933 9.13548 5.00173C9.63867 5.21016 10.0688 5.56312 10.3713 6.01598C10.6739 6.46884 10.8354 7.00125 10.8354 7.5459C10.8314 9.06689 9.59864 10.2997 8.08165 10.2997ZM28.2427 27.671H23.4957V20.2381C23.4957 18.465 23.4636 16.1875 21.0261 16.1875C18.5565 16.1875 18.1762 18.1168 18.1762 20.1101V27.671H13.4331V12.389H17.9881V14.4784H18.0521C18.6845 13.2776 20.2335 12.0088 22.547 12.0088C27.3582 12.0088 28.2427 15.1748 28.2427 19.2895V27.671Z"
                fill="#2091F9"
              />
            </svg>
          </div>
        </div>
      </div>
    </template>
    <template #footer>
      <Footer />
    </template>
  </HomepageItem>
</template>
