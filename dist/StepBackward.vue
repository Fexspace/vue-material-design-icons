<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon step-backward-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M19,5V19H16V5M14,5V19L3,12">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "StepBackwardIcon",
  props: {
    title: {
      type: String,
      default: "Step Backward icon"
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
