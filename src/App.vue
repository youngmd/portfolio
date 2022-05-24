<template>
  <div class="banner-1">
    <!-- NavBar -->
    <nav
      class="container px-6 mx-auto md:flex md:justify-between md:items-center"
    >
      <div class="flex items-center justify-between">
        <div class="relative w-24 h-24 xs:w-16 xs:h-16">
          <img
            class="rounded-full border border-gray-100 shadow-sm"
            src="./assets/headshot.png"
            alt="user image"
          />
        </div>
        <!-- Mobile menu button -->
        <div @click="showMenu = !showMenu" class="flex md:hidden">
          <button
            type="button"
            class="text-gray-800 hover:text-gray-400 focus:outline-none focus:text-gray-400"
          >
            <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
              <path
                fill-rule="evenodd"
                d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
              ></path>
            </svg>
          </button>
        </div>
      </div>
      <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
      <ul
        :class="showMenu ? 'flex' : 'hidden'"
        class="flex-col items-end mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0"
      >
        <li class="menu-button"><a href="#work" v-smooth-scroll>Recent Work</a></li>
        <li class="menu-button"><a href="#visualizations" v-smooth-scroll>Visualizations</a></li>
        <li class="menu-button"><a href="#publications" v-smooth-scroll>Publications</a></li>
        <li class="menu-button"><a href="#technologies" v-smooth-scroll>Skills</a></li>
        <li class="menu-button"><a href="#about" v-smooth-scroll>About</a></li>
      </ul>
    </nav>
    <!-- End Navbar -->

    <div class="flex items-center">
      <div class="w-11/12 space-y-6 md:space-y-10">
        <h1
          class="3xl:text-8xl 2xl:text-7xl xl:text-6xl lg:text-4xl md:text-3xl sm:text-3xl text-xl font-bold leading-tight text-gray-700"
        >
          <a
            href="https://www.linkedin.com/in/youngmd13b"
            target="_blank"
            class="text-black hover:underline"
          >
            Michael Young, Ph.D</a
          ><span class="3xl:text-6xl 2xl:text-5xl xl:text-4xl lg:text-3xl md:text-2xl sm:text-xl text-lg"><br />Data Science and Analysis<br />Full-Stack Development<br />Systems Integration</span>
        </h1>

        <div class="md:flex gap-1 md:gap-10">
          <a class="button border-4 text-white bg-gray-800 submit-button hidden md:block md:mb-0" href="#work" v-smooth-scroll>
            View My Work
          </a>
          <a
            class="text-gray-800 border-4 border-gray-800 submit-button mb-5 md:mb-0" href="mailto:jobs@youngmd.net"
          >
            Contact Me
          </a>
        </div>
      </div>

      <div class="w-8/12 flex justify-end">
        <img
          src="./assets/top_image.png"
          alt="user image"
        />
      </div>
    </div>
  </div>

  <div class="banner-2 space-y-10 pb-20" id="work">
    <h3 class="heading3 my-5">Recent Work</h3>
    <div class="card">
      <div class="space-y-5 py-8 px-8 lg:py-16 lg:px-20 lg:w-1/2">
        <h4 class="project-title item">HPC Everywhere</h4>
        <p class="font-work_sans pr-12">
          A system designed to encabsulate and abstract all of the powerful command line features available to expert HPC users and create an intuitive and accessible web-based interface that any researcher can immediately utilize to improve their HPC experience at Indiana University.
        </p>
        <button class="text-sky-800 font-bold text-2xl tracking-wider">
          View Contributions | Visit Site
        </button>
      </div>
      <div class="card-image shadow-xl mr-2">
        <img
          class="object-cover object-left-top w-full h-48 md:h-96 rounded-xl border-2"
          src="./assets/hpce_project.png"
        />
      </div>
    </div>

    <div class="card">
      <div class="card-image shadow-xl ml-2">
        <img
          class="object-cover object-left-top w-full h-48 md:h-96 rounded-xl border-2"
          src="./assets/cmg_project.png"
        />
      </div>
      <div class="space-y-5 py-8 px-8 lg:py-16 lg:px-20 lg:w-1/2">
        <h4 class="project-title item">CMG-SCA</h4>
        <p class="font-work_sans pr-12">
          Automatically archives raw sequencing data produced by genomic sequencers. Information about a run is immediately registered on the web portal so operators can monitor data archival. An integrated pipeline setup allows for conversion of the raw files to formatted data products.  Access to data products are grouped by projects that are accessible to one or more users/groups.
        </p>
        <button class="text-sky-800 font-bold text-2xl tracking-wider">
          View Contributions | Project Access Restricted
        </button>
      </div>
    </div>

    <div class="card">
      <div class="space-y-5 py-8 px-8 lg:py-16 lg:px-20 lg:w-1/2">
        <h4 class="project-title item">Electronic Health Records Dashboard</h4>
        <p class="font-work_sans pr-12">
          A system designed to encabsulate and abstract all of the powerful command line features available to expert HPC users and create an intuitive and accessible web-based interface that any researcher can immediately utilize to improve their HPC experience at Indiana University.
        </p>
        <button class="border-4 submit-button mr-2 text-sky-800 font-bold text-xl tracking-wider">
          View Contributions
        </button>
        <button class="text-sky-800 font-bold text-xl tracking-wider disabled">
          Project Access Restricted
        </button>
      </div>
      <div class="card-image mr-2 shadow-xl">
        <img
            class="object-cover object-left-top w-full h-72 md:h-96 rounded-xl border-2"
            src="./assets/ehr_project.png"
        />
      </div>
    </div>
  </div>

  <div class="banner-1" id="technologies">
    <h4 class="heading3 text-right">Skills and Technologies</h4>
    <div class="flex items-center justify-center">
      <img src="./assets/logo_cloud.png"/>
    </div>
  </div>

  <div class="banner-2" id="publications">
      <h4 class="heading3 mb-2 text-gray-200">Publications and Presentations</h4>
      <div class="text-gray-100">
        <publications :showAll="false"></publications>
      </div>
      <div class="text-right py-2">
        <button class="submit-button" id="show-modal" @click="showModal = true">Show All (37)</button>
        <Teleport to="body">
          <!-- use the modal component, pass in the prop -->
          <modal :show="showModal" @close="showModal = false">
            <template #header>
              <div class="heading4 pb-4">Publications and Presentations</div>
            </template>
            <template #body>
              <publications :showAll="true"></publications>
            </template>
          </modal>
        </Teleport>
      </div>
  </div>

  <div class="banner-1" id="visualizations">
    <div class="space-y-4 grid place-items-center mt-5">
      <h3 class="heading3">Visualizations</h3>
      <p class="font-work_sans text-gray-600 font-semibold leading-relaxed">
        Examples of data visualizations and demonstrations from various projects and papers
      </p>
    </div>
    <div class="max-w-7xl mx-auto px-8 py-16">
      <div class="relative">
        <Carousel :items-to-show="2.5" :wrap-around="true">
          <Slide v-for="slide in 10" :key="slide">
            <div class="carousel__item">{{ slide }}</div>
          </Slide>

          <template #addons>
            <Navigation />
          </template>
        </Carousel>
<!--        <Carousel :items-to-show="2.5" :wrap-around="true">-->
<!--          <Slide v-for="slide in 3" :key="slide">-->
<!--            <div class="carousel__item">-->
<!--              <div class="relative lg:flex rounded-lg shadow-2xl overflow-hidden" >-->
<!--                <div-->
<!--                    class="h-56 lg:h-auto lg:w-5/12 relative flex items-center justify-center"-->
<!--                >-->
<!--                  <img-->
<!--                      class="absolute h-full w-full object-cover"-->
<!--                      src="./assets/viz_zeropoint.png"-->
<!--                      alt=""-->
<!--                  />-->
<!--                </div>-->
<!--                <div class="relative lg:w-7/12 bg-white">-->
<!--                  <svg-->
<!--                      class="absolute h-full text-white w-24 -ml-12"-->
<!--                      fill="currentColor"-->
<!--                      viewBox="0 0 100 100"-->
<!--                      preserveAspectRatio="none"-->
<!--                  >-->
<!--                    <polygon points="50,0 100,0 50,100 0,100" />-->
<!--                  </svg>-->
<!--                  <div-->
<!--                      class="relative py-12 lg:py-24 px-8 lg:px-16 text-gray-700 leading-relaxed"-->
<!--                  >-->
<!--                    <p>-->
<!--                      Mapping fluctuations in the zeropoint magnitude of instrumental filters for the One Degree Imager, indicating a buildup of contamination.  This visualization demonstrated a need for an increased cadence of cleaning and re-aluminization, especially in the higher frequency (blue and green) filters.-->
<!--                    </p>-->
<!--                    <p class="mt-6">-->
<!--                      <a-->
<!--                          href="#"-->
<!--                          class="font-medium text-indigo-600 hover:text-indigo-900"-->
<!--                      >-->
<!--                        &rarr; MySQL, Python, HighCharts, JavaScript</a-->
<!--                      >-->
<!--                    </p>-->
<!--                  </div>-->
<!--                </div>-->
<!--              </div>-->
<!--            </div>-->
<!--          </Slide>-->

<!--          <template #addons>-->
<!--            <Navigation />-->
<!--          </template>-->
<!--        </Carousel>-->
      </div>
<!--        <div class="relative lg:flex rounded-lg shadow-2xl overflow-hidden" v-show="vizSlide == 1">-->
<!--          <div-->
<!--            class="h-56 lg:h-auto lg:w-5/12 relative flex items-center justify-center"-->
<!--          >-->
<!--            <img-->
<!--              class="absolute h-full w-full object-cover"-->
<!--              src="./assets/viz_zeropoint.png"-->
<!--              alt=""-->
<!--            />-->
<!--          </div>-->
<!--          <div class="relative lg:w-7/12 bg-white">-->
<!--            <svg-->
<!--              class="absolute h-full text-white w-24 -ml-12"-->
<!--              fill="currentColor"-->
<!--              viewBox="0 0 100 100"-->
<!--              preserveAspectRatio="none"-->
<!--            >-->
<!--              <polygon points="50,0 100,0 50,100 0,100" />-->
<!--            </svg>-->
<!--            <div-->
<!--              class="relative py-12 lg:py-24 px-8 lg:px-16 text-gray-700 leading-relaxed"-->
<!--            >-->
<!--              <p>-->
<!--                Mapping fluctuations in the zeropoint magnitude of instrumental filters for the One Degree Imager, indicating a buildup of contamination.  This visualization demonstrated a need for an increased cadence of cleaning and re-aluminization, especially in the higher frequency (blue and green) filters.-->
<!--              </p>-->
<!--              <p class="mt-6">-->
<!--                <a-->
<!--                  href="#"-->
<!--                  class="font-medium text-indigo-600 hover:text-indigo-900"-->
<!--                >-->
<!--                  &rarr; MySQL, Python, HighCharts, JavaScript</a-->
<!--                >-->
<!--              </p>-->
<!--            </div>-->
<!--          </div>-->
<!--        </div>-->
<!--        </Transition>-->
<!--        <Transition name="slide-fade">-->
<!--          <div class="relative lg:flex rounded-lg shadow-2xl overflow-hidden" v-show="vizSlide == 2">-->
<!--            <div-->
<!--                class="h-56 lg:h-96 lg:w-5/12 relative flex items-center justify-center"-->
<!--            >-->
<!--              <img-->
<!--                  class="absolute h-full w-full object-cover"-->
<!--                  src="./assets/viz_healpix.png"-->
<!--                  alt=""-->
<!--              />-->
<!--            </div>-->
<!--            <div class="relative lg:w-7/12 bg-white">-->
<!--              <svg-->
<!--                  class="absolute h-full text-white w-24 -ml-12"-->
<!--                  fill="currentColor"-->
<!--                  viewBox="0 0 100 100"-->
<!--                  preserveAspectRatio="none"-->
<!--              >-->
<!--                <polygon points="50,0 100,0 50,100 0,100" />-->
<!--              </svg>-->
<!--              <div-->
<!--                  class="relative py-12 lg:py-24 px-8 lg:px-16 text-gray-700 leading-relaxed"-->
<!--              >-->
<!--                <p>-->
<!--                  Demonstrating the performance gains of leveraging Hive partitioning to improve search performance on the Blanco DECam Bulge Survey dataset.-->
<!--                </p>-->
<!--                <p class="mt-6">-->
<!--                  <a-->
<!--                      href="#"-->
<!--                      class="font-medium text-indigo-600 hover:text-indigo-900"-->
<!--                  >-->
<!--                    &rarr; Hive, R, Spark, ggplot2</a-->
<!--                  >-->
<!--                </p>-->
<!--              </div>-->
<!--            </div>-->
<!--        </div>-->
<!--        </Transition>-->
<!--        <div class="relative lg:flex rounded-lg shadow-2xl overflow-hidden" v-show="vizSlide == 3">-->
<!--          <div-->
<!--              class="h-56 lg:h-96 lg:w-5/12 relative flex items-center justify-center"-->
<!--          >-->
<!--            <img-->
<!--                class="absolute h-full w-full object-cover"-->
<!--                src="./assets/viz_pathfinder.png"-->
<!--                alt=""-->
<!--            />-->
<!--          </div>-->
<!--          <div class="relative lg:w-7/12 bg-white">-->
<!--            <svg-->
<!--                class="absolute h-full text-white w-24 -ml-12"-->
<!--                fill="currentColor"-->
<!--                viewBox="0 0 100 100"-->
<!--                preserveAspectRatio="none"-->
<!--            >-->
<!--              <polygon points="50,0 100,0 50,100 0,100" />-->
<!--            </svg>-->
<!--            <div-->
<!--                class="relative py-12 lg:py-24 px-8 lg:px-16 text-gray-700 leading-relaxed"-->
<!--            >-->
<!--              <p>-->
<!--                Report of weighted user responses and recommendations in the Pathfinder tool, used to help guide new HPC users towards the best system for their research needs.-->
<!--              </p>-->
<!--              <p class="mt-6">-->
<!--                <a-->
<!--                    href="#"-->
<!--                    class="font-medium text-indigo-600 hover:text-indigo-900"-->
<!--                >-->
<!--                  &rarr; MySQL, JavaScript, Python, HighCharts</a-->
<!--                >-->
<!--              </p>-->
<!--            </div>-->
<!--          </div>-->
<!--        </div>-->
<!--        <div class="absolute inset-y-0 left-0 lg:flex lg:items-center">-->
<!--          <button-->
<!--            class="mt-24 lg:mt-0 -ml-6 h-12 w-12 rounded-full bg-white p-3 shadow-lg" @click="vizSlide -= 1"-->
<!--          >-->
<!--            <svg-->
<!--              class="h-full w-full text-indigo-900"-->
<!--              fill="currentColor"-->
<!--              viewBox="0 0 24 24"-->
<!--            >-->
<!--              <path-->
<!--                d="M5.41 11H21a1 1 0 0 1 0 2H5.41l5.3 5.3a1 1 0 0 1-1.42 1.4l-7-7a1 1 0 0 1 0-1.4l7-7a1 1 0 0 1 1.42 1.4L5.4 11z"-->
<!--              />-->
<!--            </svg>-->
<!--          </button>-->
<!--        </div>-->
<!--        <div class="absolute inset-y-0 right-0 lg:flex lg:items-center">-->
<!--          <button-->
<!--            class="mt-24 lg:mt-0 -mr-6 h-12 w-12 rounded-full bg-white p-3 shadow-lg" @click="vizSlide += 1"-->
<!--          >-->
<!--            <svg-->
<!--              class="h-full w-full text-indigo-900"-->
<!--              fill="currentColor"-->
<!--              viewBox="0 0 24 24"-->
<!--            >-->
<!--              <path-->
<!--                d="M18.59 13H3a1 1 0 0 1 0-2h15.59l-5.3-5.3a1 1 0 1 1 1.42-1.4l7 7a1 1 0 0 1 0 1.4l-7 7a1 1 0 0 1-1.42-1.4l5.3-5.3z"-->
<!--              />-->
<!--            </svg>-->
<!--          </button>-->
<!--        </div>-->
<!--      </div>-->
    </div>
  </div>

  <div class="banner-2 md:flex items-center md:justify-evenly bg-[url('/m51-3.jpeg')]" id="about">
    <div class="md:w-1/2">
      </div>
    <div class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-1/2">
      <div class="text-3xl text-white">About Me</div>
      <div class="font-work_sans space-y-5 space-x-5 text-white backdrop-blur backdrop-brightness-75 rounded-md">
        I am Michael Young, currently living in Bloomington, Indiana.  Though my background is that of a research astronomer,
        my current position is as the senior tech lead and principal research developer/analyst
        for the Scalable Compute Archives (SCA) team within the Research Technologies Division at Indiana University.
        <br /><br />
        Over the past decade I have collaborated and consulted with researchers, technicians, clinicians,
        and developers from a wide range of scientific and medical fields.  Working closely with these stakeholders and the SCA team, I have analyzed
        and optimized data workflows and analysis pipelines, created secure archival and metadata management systems,
        and constructed customized visualization and analysis tools.
      </div>
    </div>
  </div>

  <div class="banner-1 flex h-full items-center">
    <div class="w-7/12 p-12">
      <h2 class="text-gray-700 md:text-6xl text-2xl font-Eczar mb-5 font-bold">
        Let the data drive
      </h2>
      <a class="underline text-2xl text-blue-600 font-work_sans"
        >📧 jobs@youngmd.net</a
      >
    </div>
    <div class="w-5/12 pr-28">
      <div class="flex flex-wrap justify-end gap-2">
        <button
          class="bg-gray-700 p-2 font-semibold text-white inline-flex items-center space-x-2 rounded"
        >
          <svg
            class="w-4 h-4 md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10 fill-current"
            role="img"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
          >
            <path
              d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"
            />
          </svg>
        </button>

        <button
          class="bg-gray-700 p-2 font-semibold text-white inline-flex items-center space-x-2 rounded"
        >
          <svg
            class="w-4 h-4 md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10 fill-current"
            role="img"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
          >
            <path
              d="M23.953 4.57a10 10 0 01-2.825.775 4.958 4.958 0 002.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 00-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 00-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 01-2.228-.616v.06a4.923 4.923 0 003.946 4.827 4.996 4.996 0 01-2.212.085 4.936 4.936 0 004.604 3.417 9.867 9.867 0 01-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 007.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0024 4.59z"
            />
          </svg>
        </button>

        <button
          class="bg-gray-700 p-2 font-semibold text-white inline-flex items-center space-x-2 rounded"
        >
          <svg
            class="w-4 h-4 md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10 fill-current"
            role="img"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M12 0A12 12 0 0 0 0 12a12 12 0 0 0 12 12 12 12 0 0 0 12-12A12 12 0 0 0 12 0zm5.01 4.744c.688 0 1.25.561 1.25 1.249a1.25 1.25 0 0 1-2.498.056l-2.597-.547-.8 3.747c1.824.07 3.48.632 4.674 1.488.308-.309.73-.491 1.207-.491.968 0 1.754.786 1.754 1.754 0 .716-.435 1.333-1.01 1.614a3.111 3.111 0 0 1 .042.52c0 2.694-3.13 4.87-7.004 4.87-3.874 0-7.004-2.176-7.004-4.87 0-.183.015-.366.043-.534A1.748 1.748 0 0 1 4.028 12c0-.968.786-1.754 1.754-1.754.463 0 .898.196 1.207.49 1.207-.883 2.878-1.43 4.744-1.487l.885-4.182a.342.342 0 0 1 .14-.197.35.35 0 0 1 .238-.042l2.906.617a1.214 1.214 0 0 1 1.108-.701zM9.25 12C8.561 12 8 12.562 8 13.25c0 .687.561 1.248 1.25 1.248.687 0 1.248-.561 1.248-1.249 0-.688-.561-1.249-1.249-1.249zm5.5 0c-.687 0-1.248.561-1.248 1.25 0 .687.561 1.248 1.249 1.248.688 0 1.249-.561 1.249-1.249 0-.687-.562-1.249-1.25-1.249zm-5.466 3.99a.327.327 0 0 0-.231.094.33.33 0 0 0 0 .463c.842.842 2.484.913 2.961.913.477 0 2.105-.056 2.961-.913a.361.361 0 0 0 .029-.463.33.33 0 0 0-.464 0c-.547.533-1.684.73-2.512.73-.828 0-1.979-.196-2.512-.73a.326.326 0 0 0-.232-.095z"
            />
          </svg>
        </button>

        <button
          class="bg-gray-700 p-2 font-semibold text-white inline-flex items-center space-x-2 rounded"
        >
          <svg
            class="w-4 h-4 md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10 fill-current"
            role="img"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M12.017 0C5.396 0 .029 5.367.029 11.987c0 5.079 3.158 9.417 7.618 11.162-.105-.949-.199-2.403.041-3.439.219-.937 1.406-5.957 1.406-5.957s-.359-.72-.359-1.781c0-1.663.967-2.911 2.168-2.911 1.024 0 1.518.769 1.518 1.688 0 1.029-.653 2.567-.992 3.992-.285 1.193.6 2.165 1.775 2.165 2.128 0 3.768-2.245 3.768-5.487 0-2.861-2.063-4.869-5.008-4.869-3.41 0-5.409 2.562-5.409 5.199 0 1.033.394 2.143.889 2.741.099.12.112.225.085.345-.09.375-.293 1.199-.334 1.363-.053.225-.172.271-.401.165-1.495-.69-2.433-2.878-2.433-4.646 0-3.776 2.748-7.252 7.92-7.252 4.158 0 7.392 2.967 7.392 6.923 0 4.135-2.607 7.462-6.233 7.462-1.214 0-2.354-.629-2.758-1.379l-.749 2.848c-.269 1.045-1.004 2.352-1.498 3.146 1.123.345 2.306.535 3.55.535 6.607 0 11.985-5.365 11.985-11.987C23.97 5.39 18.592.026 11.985.026L12.017 0z"
            />
          </svg>
        </button>

      </div>
    </div>
  </div>
</template>
<script setup>
import { ref } from 'vue'
import Publications from "./publications.vue";
import Modal from './modal.vue';

import 'vue3-carousel/dist/carousel.css';
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel';

const showModal = ref(false)
const showMenu = ref(false)

const vizSlide = ref(1)

const skills = {
  'Languages': 'Python, R, JavaScript, PHP',
  'Databases': 'MySQL, PostgreSQL, Mongo, Hive, Oracle',
  'Visualization': 'Tableau, ggplot2, d3.js, Highcharts, matplotlib',
  'Libraries': 'NumPy, SciPy, pandas, Scikit-learn, Tensorflow',
  'Statistical Methods': 'Mixture Modeling, Monte Carlo Markov Chains, Time Series Forecasting',
  'Other': 'Docker, Kubernetes, AWS, Azure, GitHub, JIRA, Hadoop/HDFS/Spark, Google Analytics'
}

</script>

<style>
/*
  Enter and leave animations can use different
  durations and timing functions.
*/
.slide-fade-enter-active {
  transition: all 0.3s ease-out;
}

.slide-fade-enter-from {
  transform: translateX(20px);
  opacity: 0;
}

</style>
