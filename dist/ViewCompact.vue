<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon view-compact-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M3,19H9V12H3V19M10,19H22V12H10V19M3,5V11H22V5H3Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ViewCompactIcon",
  props: {
    title: {
      type: String,
      default: "View Compact icon"
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
