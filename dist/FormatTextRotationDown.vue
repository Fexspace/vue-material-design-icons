<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon format-text-rotation-down-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M6,19.73L3,16.73H5V4.27H7V16.73H9L6,19.73M14,9.38V13.13L19.03,11.25L14,9.38M21,12L10,16.73V14.67L12.19,13.73V8.77L10,7.83V5.77L21,10.5V12Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FormatTextRotationDownIcon",
  props: {
    title: {
      type: String,
      default: "Format Text Rotation Down icon"
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
