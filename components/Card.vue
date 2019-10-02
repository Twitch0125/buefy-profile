<template>
  <div class="column">
    <div class="card">
      <header class="card-header">
        <p class="card-header-title has-text-primary">{{ title }}</p>
      </header>
      <div class="card-image lottie primary flex">
        <div class="image has-text-centered">
          <slot name="lottie" />
        </div>
      </div>
      <section class="card-content description">
        <div class="content">
          <slot name="description" />
        </div>
      </section>
      <footer class="card-footer">
        <div class="card-footer-item level">
          <div class="level-left">
            <div class="level-item">
              <b-button
                tag="a"
                :href="github"
                target="new"
                type="is-primary"
                size="is-medium"
                icon-left="github-circle"
              >Github</b-button>
            </div>
          </div>
          <div class="level-right">
            <div class="level-item">
              <b-button tag="a" target="new" :href="host" type="is-primary" size="is-medium">Visit</b-button>
            </div>
          </div>
        </div>
      </footer>
    </div>
  </div>
</template>

<style lang="scss">
@import "~assets/css/styles.scss";

.flex {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.lottie {
  width: 300px;
  height: 300px;
}
.description {
  width: 300px;
  height: 144px;
}
.primary {
  background-color: $primary;
}
.primary-text {
  color: $primary-invert;
}
</style>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    icon: {
      type: String,
      required: true
    },
    github: {
      type: String,
      required: false
    },
    host: {
      type: String,
      required: false
    }
  }
};
</script>
