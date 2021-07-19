<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon facebook-gaming-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M9.5 14.5V9.5H21V21H15.5V14.5H9.5M3 3H21L21 8.5H8.5V15.5H14.5V21H3V3Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FacebookGamingIcon",
  props: {
    title: {
      type: String,
      default: "Facebook Gaming icon"
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
