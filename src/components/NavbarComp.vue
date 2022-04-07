<template>
  <div>
    <b-navbar toggleable="lg" type="light" variant="light" class="p-3">
      <b-navbar-brand to="/">Mi App</b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav class="justify-content-end">
        <b-navbar-nav>
          <b-nav-item to="/">INICIO</b-nav-item>
          <b-nav-item class="mx-2" to="/buscar">BUSCAR</b-nav-item>
          <b-nav-item to="/about">ACERCA DE</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "NavbarComp",
};
</script>

<style>
nav {
  border-bottom: 4px groove #aba6a6;
}
</style>
