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
          <a class="button border-4 text-white bg-gray-800 submit-button hidden md:block md:mb-0" href="#about" v-smooth-scroll>
            About Me
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
    <h3 class="heading3 my-5 text-sky-800">Recent Work</h3>

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
        <button class="text-sky-800 font-bold text-xl tracking-wider disabled">
          Project Access Restricted
        </button>
      </div>
    </div>

    <div class="card">
      <div class="space-y-5 py-8 px-8 lg:py-16 lg:px-20 lg:w-1/2">
        <h4 class="project-title item">HPC Everywhere</h4>
        <p class="font-work_sans pr-12">
          A system designed to encabsulate and abstract all of the powerful command line features available to expert HPC users and create an intuitive and accessible web-based interface that any researcher can immediately utilize to improve their HPC experience at Indiana University.
        </p>
        <div class="md:flex gap-1 md:gap-10">
        <a class="btn border-4 border-gray-800 submit-button text-sky-800 font-bold text-2xl tracking-wider" href="https://hpceverywhere.iu.edu" target="_blank">
          Visit Site
        </a>
          </div>
      </div>
      <div class="card-image shadow-xl mr-2">
        <img
          class="object-cover object-left-top w-full h-48 md:h-96 rounded-xl border-2"
          src="./assets/hpce_project.png"
        />
      </div>
    </div>

    <div class="card">
      <div class="card-image mr-2 shadow-xl">
        <img
            class="object-cover object-left-top w-full h-72 md:h-96 rounded-xl border-2"
            src="./assets/ehr_project.png"
        />
      </div>
      <div class="space-y-5 py-8 px-8 lg:py-16 lg:px-20 lg:w-1/2">
        <h4 class="project-title item">Electronic Health Records Dashboard</h4>
        <p class="font-work_sans pr-12">
          Working with a partner institution I developed a prototype dashboard which collates patient records across years of visits and displays and groups these records based on a proprietary relevance grouping API.
        </p>

        <button class="text-sky-800 font-bold text-xl tracking-wider disabled">
          Project Access Restricted
        </button>
      </div>
    </div>

    <div class="text-right py-2">
      <a class="submit-button" href="https://sca.iu.edu/person/youngmd" target="_blank">See More</a>
    </div>
  </div>

  <div class="banner-1" id="visualizations">
    <div class="space-y-4 grid place-items-center mt-5">
      <h3 class="heading3a">Visualizations</h3>
      <p class="font-work_sans text-gray-600 font-semibold leading-relaxed">
        Examples of data visualizations and demonstrations from various projects and papers
      </p>
    </div>
    <div class="max-w-7xl mx-auto px-8 py-16">
      <div class="relative">
        <Carousel :autoplay="9000" :items-to-show="1" :wrap-around="true">
          <Slide v-for="slide in 5" :key="slide">
            <div class="carousel__item"><Viz :showVis="slide - 1"></Viz> </div>
          </Slide>

          <template #addons>
            <Navigation />
          </template>
        </Carousel>
      </div>
    </div>
  </div>

  <div class="banner-2" id="publications">
      <h4 class="heading3 mb-2 text-gray-200">Publications and Presentations</h4>
      <div class="text-gray-100">
        <publications :showAll="false"></publications>
      </div>
      <div class="text-right py-2">
        <button class="submit-button" id="show-modal" @click="showModal = true">Show All (21)</button>
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

  <div class="banner-1" id="technologies">
    <h4 class="heading3a text-right">Skills and Technologies</h4>
    <div class="flex items-center justify-center">
      <img src="./assets/logo_cloud.png"/>
    </div>
  </div>

  <div class="banner-2 md:flex items-center md:justify-evenly bg-[url('/m51-3.jpeg')]" id="about">
    <div class="md:w-1/2">
      </div>
    <div class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-1/2">
      <div class="text-3xl text-white">About Me</div>
      <div class="font-work_sans space-y-5 space-x-5 text-white backdrop-blur backdrop-brightness-75 rounded-md">
        I am Michael Young, currently living in Bloomington, Indiana.  With a background as a published observational astronomer,
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

      <div>
        <a class="font-work_sans text-gray-600 font-semibold leading-relaxed text-3xl" href="mailto:jobs@youngmd.net"
        ><Mail /> jobs@youngmd.net</a
        >
      </div>
      <div>
        <a class="font-work_sans text-gray-600 font-semibold leading-relaxed text-3xl" href="https://github.com/youngmd" target="_blank"
        ><Github /> github.com/youngmd</a
        >
      </div>
      <div>
        <a class="font-work_sans text-gray-600 font-semibold leading-relaxed text-3xl" href="https://www.linkedin.com/in/youngmd13b/" target="_blank"
        ><Linkedin /> linkedin.com/in/youngmd13b</a
        >
      </div>
    </div>
  </div>
</template>
<script setup>
import { ref } from 'vue'
import Publications from "./publications.vue";
import Viz from './Viz.vue';
import Modal from './modal.vue';

import 'vue3-carousel/dist/carousel.css';
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel';
import 'vue-material-design-icons/styles.css';
import Mail from 'vue-material-design-icons/Mail.vue'
import Github from 'vue-material-design-icons/Github.vue'
import Linkedin from 'vue-material-design-icons/Linkedin.vue'

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

.carousel__prev,
.carousel__next {
  color: gray;
  box-sizing: content-box;
  border: 4px solid gray;
}

</style>
