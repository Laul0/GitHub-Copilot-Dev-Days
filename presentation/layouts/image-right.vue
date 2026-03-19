<script setup lang="ts">
import { computed } from 'vue'

const props = defineProps({
  image: { type: String },
  class: { type: String },
  // default is 'contain' — same as Marp's "fit" keyword
  backgroundSize: { type: String, default: 'contain' },
  // column width for the image — mirrors Marp's right:40%
  imageWidth: { type: String, default: '40%' },
})

const gridStyle = computed(() => ({
  gridTemplateColumns: `1fr ${props.imageWidth}`,
}))

const imageStyle = computed(() => ({
  backgroundImage: props.image ? `url("${props.image}")` : undefined,
  backgroundRepeat: 'no-repeat',
  backgroundPosition: 'center',
  backgroundSize: props.backgroundSize,
}))
</script>

<template>
  <div class="grid w-full h-full" :style="gridStyle">
    <div class="slidev-layout default overflow-hidden" :class="props.class">
      <slot />
    </div>
    <div class="w-full h-full" :style="imageStyle" />
  </div>
</template>
