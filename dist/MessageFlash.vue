<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon message-flash-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M22 4C22 2.9 21.1 2 20 2H4C2.9 2 2 2.9 2 4V22L6 18H15V10H22V4M22.5 16H20.3L22 12H17V18H19V23L22.5 16Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "MessageFlashIcon",
  props: {
    title: {
      type: String,
      default: "Message Flash icon"
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
