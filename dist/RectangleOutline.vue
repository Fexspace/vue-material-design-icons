<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon rectangle-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M4,6V19H20V6H4M18,17H6V8H18V17Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "RectangleOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Rectangle Outline icon"
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
