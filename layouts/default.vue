<script lang="ts" setup>
import type { LenisOptions } from "lenis";

import { VueLenis } from "lenis/vue";

const lenisOptions: LenisOptions = {
  orientation: "vertical",
  smoothWheel: true,
  duration: 1,
  wheelMultiplier: 1.5,
  // lerp: 0.99,
};
</script>

<template>
  <VueLenis root :option="lenisOptions">
    <AppHeader />
    <main>
      <slot />
    </main>
    <AppFooter />
  </VueLenis>
</template>
