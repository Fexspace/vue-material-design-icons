<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon send-check-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M2 3V10L17 12L2 14V21L23 12M4 6.03L11.53 9.25L4 8.25M11.53 14.75L4 17.97V15.75M22 15.5L18.5 19L16.5 17L15 18.5L18.5 22L23.5 17Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SendCheckOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Send Check Outline icon"
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
