<template>
  <div class="home">
    <Figma :figma="figmaConfig" v-model="viewModel" :config="config"/>
  </div>
</template>


<script>
import Vue from "vue";
import Figma from "vue-low-code";
Vue.use(Figma);

// import JSON file for deployment
// import app from './app.json'

export default {
  name: "Home",
  data: function () {
    return {
      // figmaJSON: app,
      figmaConfig: {
        figmaFile: "ppOUWhTKkTv1oGxZp2QPrf",
        figmaAccessKey: "197735-bae0ce50-c4fd-4b30-9334-a0c0044294a0",
      },
      viewModel: {
        /**
         * Add your view model here
         */
      },
      config: {
        responsive: [
          { value: "Desktop", label: "Desktop", types: ["desktop"] },
          { value: "Mobile", label: "Mobile", types: ["tablet", "mobile"] },
        ],
        components: {
          /**
           * Register costum components here
           */
        },
      },
    };
  },
  components: {},
  methods: {
    /**
     * Place your methods here
     */
  },
};
</script>
