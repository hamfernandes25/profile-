<template>
  <p><b>Educational Qualifications</b></p>
  <v-timeline align="start">
    <v-timeline-item
      v-for="(year, i) in years"
      :key="i"
      :dot-color="year.color"
      size="small"
    >
      <template v-slot:opposite>
        <div
          :class="`pt-1 headline font-weight-bold text-${year.color}`"
          v-text="year.year"
        ></div>
      </template>
      <div>
        <h2 :class="`mt-n1 headline font-weight-light mb-4 text-${year.color}`">
          {{ year.title }}
        </h2>
        <div>
          {{ year.desc1 }}
        </div>
        <div>
          {{ year.desc2 }}
        </div>
      </div>
      <div>
        {{ year.desc3 }}
      </div>
    </v-timeline-item>
  </v-timeline>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
//import CardView from './card.vue'

export default {
  name: "TImeLine",
  components: {
    // HelloWorld,
    // CardView,
  },
  data: () => ({
    years: [
      {
        color: "cyan",
        year: "2013- 2017",
        title: "Under-Graduate Degree ",
        desc1: "Bachelor of Engineering (BE)",
        desc2:
          " Information Technology Goa College of Engineering (Goa University) – India  ",
        desc3:
          "  Grade: First Class with Distinction - 71.26% (5th to 8th semester)",
      },
      {
        color: "green",
        year: "2011– 2013 ",
        title: "Higher Secondary School ",
        desc1:
          "Fr. Agnel Multipurpose Higher Secondary School – Verna, Goa, India  ",
        desc2: " Subjects: Physics, Chemistry, Mathematics, Geology ",
        desc3: " Grade: First Class - 71.5%",
      },
      {
        color: "red",
        year: "2005-2011",
        title: "Secondary School (Class 5 – Class 10)  ",
        desc1: "St. Jude’s High School – Betalbatim, Goa, India  ",
        desc2: " Subjects: English, Mathematics, Science  ",
        desc3: " Class 10 Final Percentage: 79.5%",
      },
    ],
  }),
};
</script>
