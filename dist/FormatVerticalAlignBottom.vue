<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon format-vertical-align-bottom-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M16,13H13V3H11V13H8L12,17L16,13M4,19V21H20V19H4Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FormatVerticalAlignBottomIcon",
  props: {
    title: {
      type: String,
      default: "Format Vertical Align Bottom icon"
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
