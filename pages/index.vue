<template>
  <section class="section">
    <div class="columns">
      <card
        title="React Mock Ecommerce"
        icon="rocket"
        github="https://github.com/Twitch0125/ecommerce"
        host="https://twitch0125.github.io/ecommerce/"
      >
        <template slot="lottie">
          <lottie-player
            src="https://assets8.lottiefiles.com/datafiles/qUMDy7X7Pw2SttP/data.json"
            background="#00DEAF"
            speed="1"
            loop
            autoplay
          ></lottie-player>
        </template>
        <template slot="description">
          <span
            class="is-family-primary"
          >My react ecommerce site was my first project using React. I used Material-UI for the UI, and Redux for state management</span>
        </template>
      </card>

      <card
        title="PostgreSQL/MongoDB CRUD"
        icon="rocket"
        github="https://github.com/Twitch0125/user-manager-postgresql"
        host="https://enigmatic-forest-13135.herokuapp.com/"
      >
        <template slot="lottie">
          <lottie-player
            src="https://assets5.lottiefiles.com/packages/lf20_ZWEJL5.json"
            background="#00DEAF"
            speed="1"
            loop
            autoplay
          ></lottie-player>
        </template>
        <template slot="description">
          <span
            class="is-family-primary"
          >Simple NodeJS user manager for PostgreSQL and MongoDB. Server Side Rendered. Templating with Pug (formerly Jade)</span>
        </template>
      </card>

      <card
        title="Angular/Ionic Giphy Chat"
        icon="rocket"
        github="https://github.com/Twitch0125/team-5-giphy-chat"
        host="https://team-5-giphy-chat.web.app/welcome"
      >
        <template slot="lottie">
          <lottie-player
            src="https://assets6.lottiefiles.com/packages/lf20_0bHF6f.json"
            background="#00DEAF"
            speed="1"
            loop
            autoplay
          ></lottie-player>
        </template>
        <template slot="description">
          <span class="is-family-primary">
            This was made with Ionic and Angular, made specifically for Mobile devices so desktop looks weird.
            It was also a group project ran with Agile principles.
          </span>
        </template>
      </card>

      <card title="Ionic Golf Scorecard" icon="rocket">
        <template slot="lottie">
          <div class="center-icon">
            <b-icon type="is-white" size="is-large" icon="rocket"></b-icon>
          </div>
        </template>
        <template slot="description">
          <span
            class="is-family-primary"
          >My first Angular project. I started this to learn Angular, and later switched to Ionic as it simplified many things (meant for mobile devices)</span>
        </template>
      </card>
    </div>
    <article class="message is-primary">
      <div class="message-header">
        <p>But wait, there's more!</p>
      </div>
      <div class="message-body message-background-color">
        This site is still a work-in-progress, so it may have some "unintended features" still. I'll put more projects on as I have time, and when I complete more. Feel free to contact me here:
        <a
          href="mailto:twitcherc@gmail.com"
          target="new"
        >twitcherc@gmail.com</a> and
        <a href="https://www.linkedin.com/in/kaleb-e/" target="new">here</a>
        <br />
        <br />
        <span class="is-family-monospace">
          Just in case you were wondering... this site was made with the amazing
          <a
            href="https://bulma.io/"
            target="new"
          >Bulma</a> and
          <a href="https://buefy.org/" target="new">Buefy</a> css frameworks. Created with
          <a href="https://vuejs.org/" target="new">Vue.js</a> and
          <a href="https://nuxtjs.org/" target="new">Nuxt.js</a>
        </span>
      </div>
    </article>
  </section>
</template>
<style lang="scss" scoped>
.center-icon {
  width: 100%;
  height: 100%;
}
.message-background-color {
  background-color: #e6fffa;
}
</style>

<script>
import Card from "~/components/Card";

export default {
  name: "HomePage",

  components: {
    Card
  }
};
</script>
