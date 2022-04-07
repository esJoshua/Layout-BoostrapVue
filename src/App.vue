<template>
  <div>
    <Navbar />
    <RouterView />
  </div>
</template>

<script>
import Navbar from "@/components/NavbarComp.vue";
import { mapState } from "vuex";

export default {
  name: "App",
  created() {
    this.personajes;
  },
  computed: {
    ...mapState(["personajes"]),
  },
  components: {
    Navbar,
  },
};
</script>
