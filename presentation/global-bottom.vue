<script setup lang="ts">
import { computed } from 'vue'
import { useSlideContext } from '@slidev/client'

const { $page, $nav, $slidev, $frontmatter } = useSlideContext()
const total = computed(() => $nav.value.total)
const hide = computed(() => {
  const cls = String($frontmatter.class ?? '')
  return cls.includes('section-break') || cls.includes('cover-slide') || cls.includes('end-slide')
})
</script>

<template>
  <template v-if="!hide && $slidev.configs.paginate && $page > 0">
    <div class="slide-footer">
      GitHub Copilot Dev Days · Montréal · 19 mars 2026
    </div>
    <div class="slide-page-num">
      {{ $page }} / {{ total }}
    </div>
  </template>
</template>

<style scoped>
.slide-footer {
  position: fixed;
  bottom: 14px;
  left: 56px;
  font-size: 0.52em;
  color: #8b949e;
  font-family: 'Inter', -apple-system, sans-serif;
  z-index: 100;
  pointer-events: none;
}
.slide-page-num {
  position: fixed;
  bottom: 14px;
  right: 18px;
  font-size: 0.52em;
  color: #8b949e;
  font-family: 'Inter', -apple-system, sans-serif;
  z-index: 100;
  pointer-events: none;
  letter-spacing: 0.03em;
}
</style>
