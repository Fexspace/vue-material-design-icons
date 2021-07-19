<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon lightning-bolt-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M11 15H6L13 1V9H18L11 23V15Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "LightningBoltIcon",
  props: {
    title: {
      type: String,
      default: "Lightning Bolt icon"
    },
    decorative: {
      type: Boolean,
      default: false
    },
    fillColor: {
      type: String,
      default: "currentColor"
    },
    size: {
      type: Number,
      default: 24
    }
  }
}
</script>
