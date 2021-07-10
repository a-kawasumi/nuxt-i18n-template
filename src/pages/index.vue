<template>
  <div class="flex flex-col">
    <div>{{ message }}</div>
    <nuxt-link :to="switchLocalePath('en')">English</nuxt-link>
    <nuxt-link :to="switchLocalePath('jp')">日本語</nuxt-link>
    <nuxt-link :to="localePath('sample')"> to sample page </nuxt-link>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "nuxt-property-decorator";

@Component
export default class PagesIndex extends Vue {
  message = this.$t("welcome");
}
</script>

<style></style>
