<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon skip-forward-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M4,5V19L11,12M18,5V19H20V5M11,5V19L18,12">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SkipForwardIcon",
  props: {
    title: {
      type: String,
      default: "Skip Forward icon"
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
