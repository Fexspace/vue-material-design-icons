<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon send-check-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M2 3V10L17 12L2 14V21L23 12M22 15.5L18.5 19L16.5 17L15 18.5L18.5 22L23.5 17Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SendCheckIcon",
  props: {
    title: {
      type: String,
      default: "Send Check icon"
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
