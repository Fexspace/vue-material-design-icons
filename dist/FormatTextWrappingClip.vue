<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon format-text-wrapping-clip-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M7,21H5V3H7V21M17,3V11H9V13H17V21H19V3H17Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FormatTextWrappingClipIcon",
  props: {
    title: {
      type: String,
      default: "Format Text Wrapping Clip icon"
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
