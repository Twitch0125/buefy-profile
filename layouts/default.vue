<template>
  <div>
    <!-- lottie player -->
    <script defer src="https://unpkg.com/@lottiefiles/lottie-player@latest/dist/lottie-player.js"></script>
    <!-- navbar -->
    <b-navbar type="is-primary" shadow>
      <template slot="start">
        <b-navbar-item tag="router-link" :to="{path: '/'}">Home</b-navbar-item>
        <!-- <b-navbar-item tag="router-link" :to="{path: '/about'}">Who am I?</b-navbar-item> -->
      </template>
      <template slot="brand">
        <b-navbar-item tag="router-link" :to="{path: '/'}">Kaleb Ercanbrack</b-navbar-item>
      </template>
      <template slot="end">
        <b-navbar-item>
          <a
            style="color: black"
            href="mailto:twitcherc@gmail.com"
            target="blank"
          >twitcherc@gmail.com</a>
        </b-navbar-item>
        <b-navbar-item>
          <b-button
            type="is-primary"
            size="is-medium"
            icon-left="github-circle"
            tag="a"
            href="https://www.github.com/Twitch0125"
            target="new"
          >Github</b-button>
        </b-navbar-item>
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
        }
      ]
    };
  }
};
</script>
