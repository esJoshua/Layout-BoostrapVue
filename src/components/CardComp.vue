<template>
  <div>
    <b-container class="mt-3">
      <b-row class="justify-content-space">
        <b-col v-for="personaje in dataPersonajes" :key="personaje.id" md="4">
          <b-card
            :title="personaje.nombre"
            :img-src="personaje.imagen"
            :img-alt="personaje.nombre"
            bg-variant="light"
            text-variant="white"
            class="my-1"
          >
          </b-card>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: "CardComp",
  props: {
    dataPersonajes: {
      type: Array,
      default: () => [],
    },
  },
};
</script>
