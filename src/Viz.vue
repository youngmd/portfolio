<script setup>
import { ref, computed } from 'vue'

const props = defineProps({
  showVis: Number
})

const visuals = ref([
  {
    img: "/viz_mm.png",
    desc: "Gaussian mixture-model testing.  Used a bootstrap method to generate and test a likelihood that the observed colors (metallicity) of a particular globular cluster population could best be explained by a mixture of two or three normal distributions.",
    skills: 'R, JAGS, ggplot2'
  },
  {
    img: "/viz_zeropoint.png",
    desc: "Mapping fluctuations in the zeropoint magnitude of instrumental filters for the One Degree Imager, indicating a buildup of contamination.  This visualization demonstrated a need for an increased cadence of cleaning and re-aluminization, especially in the higher frequency (blue and green) filters.",
    skills: 'MySQL, Python, HighCharts, JavaScript'
  },
  {
    img: "/viz_healpix.png",
    desc: "Demonstrating the performance gains of leveraging Hive partitioning to improve search performance on the Blanco DECam Bulge Survey dataset."
    ,skills: 'Hive, Python, R, Spark'
  },
  {
    img: "/viz_pathfinder.png",
    desc: "Report of weighted user responses and recommendations in the Pathfinder tool, used to help guide new HPC users towards the best system for their research needs.",
    skills: 'MongoDB, d3.js, VueJS, JavaScript, Bootstrap'
  },
  {
    img: "/viz_hew.png",
    desc: "Tableau report of high-performance computing user acquisition and behavior, with time-of-day and year analysis.  Created pipelines to automatically extract and transform data daily to generate reports",
    skills: 'Tableau, MongoDB, JavaScript'
  }
])

const visual = computed(() => {
  return visuals.value[props.showVis]
})
</script>

<template>
    <div class="relative lg:flex rounded-lg overflow-hidden">
      <div
        class="h-56 lg:h-auto lg:w-5/12 relative flex items-center justify-center"
      >
        <img
          class="absolute h-full w-full object-cover"
          :src="visual.img"
          alt=""
        />
      </div>
      <div class="relative lg:w-7/12 bg-white">
        <svg
          class="absolute h-full text-white w-24 -ml-12"
          fill="currentColor"
          viewBox="0 0 100 100"
          preserveAspectRatio="none"
        >
          <polygon points="50,0 100,0 50,100 0,100" />
        </svg>
        <div
          class="relative py-12 lg:py-24 px-8 lg:px-16 text-gray-700 leading-relaxed"
        >
          <p class="text-left">{{visual.desc}}</p>
          <p class="mt-6">
            <a
              href="#"
              class="font-medium text-indigo-600 hover:text-indigo-900"
            >
              &rarr; {{visual.skills}}</a
            >
          </p>
        </div>
      </div>
    </div>

</template>
