<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon format-text-rotation-down-vertical-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M15.25 4H13.75L9 15H11.1L12 12.8H17L17.9 15H20L15.25 4M12.63 11L14.5 6L16.37 11H12.63M5 17.5L8 14.5H6V2H4V14.5H2L5 17.5M22 20L19 17V19H6.5V21H19V23L22 20Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FormatTextRotationDownVerticalIcon",
  props: {
    title: {
      type: String,
      default: "Format Text Rotation Down Vertical icon"
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
