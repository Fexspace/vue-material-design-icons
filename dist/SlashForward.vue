<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon slash-forward-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M7 21L14.9 3H17L9.1 21H7Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SlashForwardIcon",
  props: {
    title: {
      type: String,
      default: "Slash Forward icon"
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
