<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon skip-previous-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M6,18V6H8V18H6M9.5,12L18,6V18L9.5,12Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SkipPreviousIcon",
  props: {
    title: {
      type: String,
      default: "Skip Previous icon"
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
