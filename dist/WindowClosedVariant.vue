<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon window-closed-variant-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M21 20V2H3V20H1V23H23V20M19 4V11H13V4M5 4H11V11H5M5 20V13H11V20M13 20V13H19V20Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "WindowClosedVariantIcon",
  props: {
    title: {
      type: String,
      default: "Window Closed Variant icon"
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
