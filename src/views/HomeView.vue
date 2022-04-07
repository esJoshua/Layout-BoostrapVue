<template>
  <Card :dataPersonajes="personajes" />
</template>

<script>
import Card from "@/components/CardComp.vue";
import { mapState } from "vuex";

export default {
  name: "HomeView",
  computed: {
    ...mapState(["personajes"]),
  },
  components: {
    Card,
  },
};
</script>

<style>
* {
  color: black;
  font-weight: bold;
}
</style>
