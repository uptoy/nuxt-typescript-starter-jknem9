<template>
  <div class="container">
    <div>
      <Logo />
      <h1 class="title">{{ title }}</h1>
      <div class="links">
        <a
          href="https://typescript.nuxtjs.org/"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          Documentation
        </a>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';
@Component({})
export default class Home extends Vue {
  title: string = '';
  created() {
    this.title = 'Nuxt TypeScript';
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
