<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon step-backward2-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M17,5H14V19H17V5M12,5L1,12L12,19V5M22,5H19V19H22V5Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "StepBackward2Icon",
  props: {
    title: {
      type: String,
      default: "Step Backward2 icon"
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
