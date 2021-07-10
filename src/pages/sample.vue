<template>
  <div class="flex flex-col">
    <h1>{{ $t("welcome") }}</h1>
    <nuxt-link :to="localePath('index')"> to index page </nuxt-link>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "nuxt-property-decorator";

@Component
export default class PagesIndex extends Vue {}
</script>

<style></style>
