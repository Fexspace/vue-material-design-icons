<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon format-text-rotation-vertical-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M15.75 5H14.25L9.5 16H11.6L12.5 13.8H17.5L18.4 16H20.5L15.75 5M13.13 12L15 7L16.87 12H13.13M6 19.75L9 16.75H7V4.25H5V16.75H3L6 19.75Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FormatTextRotationVerticalIcon",
  props: {
    title: {
      type: String,
      default: "Format Text Rotation Vertical icon"
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
