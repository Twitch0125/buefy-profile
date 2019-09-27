<template>
  <div>
    <!-- navbar -->
    <b-navbar type="is-primary" shadow="true">
      <template slot="start">
        <b-navbar-item tag="router-link" :to="{path: '/'}">Home</b-navbar-item>
        <b-navbar-item tag="router-link" :to="{path: '/about'}">Who am I?</b-navbar-item>
      </template>
      <template slot="brand">
        <b-navbar-item tag="router-link" :to="{path: '/'}">Home</b-navbar-item>
      </template>
    </b-navbar>

    <div class="container column is-10">
      <nuxt />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: "Home",
          icon: "home",
          to: { name: "index" }
        },
        {
          title: "Inspire",
          icon: "lightbulb",
          to: { name: "inspire" }
        }
      ]
    };
  }
};
</script>
