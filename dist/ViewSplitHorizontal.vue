<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon view-split-horizontal-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M3,5H21V7H3V5M3,11V9H21V11H3M3,19V13H21V19H3Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ViewSplitHorizontalIcon",
  props: {
    title: {
      type: String,
      default: "View Split Horizontal icon"
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
