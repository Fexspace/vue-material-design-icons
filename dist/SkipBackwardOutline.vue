<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon skip-backward-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M18,14.17L15.83,12L18,9.83V14.17M20,19V5L13,12M4,19H6V5H4M11,14.17L8.83,12L11,9.83V14.17M13,19V5L6,12">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SkipBackwardOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Skip Backward Outline icon"
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
