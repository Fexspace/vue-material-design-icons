<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon format-horizontal-align-left-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M11,16V13H21V11H11V8L7,12L11,16M3,20H5V4H3V20Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FormatHorizontalAlignLeftIcon",
  props: {
    title: {
      type: String,
      default: "Format Horizontal Align Left icon"
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
