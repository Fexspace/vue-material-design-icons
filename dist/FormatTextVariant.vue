<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon format-text-variant-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M9.6,14L12,7.7L14.4,14M11,5L5.5,19H7.7L8.8,16H15L16.1,19H18.3L13,5H11Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FormatTextVariantIcon",
  props: {
    title: {
      type: String,
      default: "Format Text Variant icon"
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
