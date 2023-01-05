<script>
import { mapState } from "vuex";
export default {
  data: () => {
    return {
      // @todo
    };
  },
  computed: {
    ...mapState(["clientsHeading", "clients"]),
  },
};
</script>

<template></template>
