<script>
import { mapState } from "vuex";

export default {
  data: () => {
    return {
      projectName: "DEVPROMISE PORTFOLIO",
      author: "DEVPROMISE",
    };
  },
  computed: {
    currentYear() {
      return new Date().getFullYear();
    },
  },
};
</script>

<template>
  <div class="flex justify-center items-center text-center">
    <div
      class="
        font-general-regular
        text-lg text-ternary-dark
        dark:text-ternary-light
      "
    >
      {{ currentYear }}.
      <a
        href="https://github.com/eziamakapromise"
        target="__blank"
        class="
          font-general-medium
          hover:underline hover:text-indigo-600
          dark:hover:text-indigo-300
          duration-500
        "
        >{{ projectName }}</a
      >
      . Developed by
      <a
        href="https://www.linkedin.com/in/promise-tobe-eziamaka-06297a248/"
        target="__blank"
        class="
          font-general-medium
          text-secondary-dark
          dark:text-secondary-light
          uppercase
          hover:underline hover:text-indigo-600
          dark:hover:text-indigo-300
          duration-500
        "
        >{{ author }}</a
      >
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
