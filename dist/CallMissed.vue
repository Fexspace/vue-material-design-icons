<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon call-missed-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M19.59,7L12,14.59L6.41,9H11V7H3V15H5V10.41L12,17.41L21,8.41">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "CallMissedIcon",
  props: {
    title: {
      type: String,
      default: "Call Missed icon"
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
