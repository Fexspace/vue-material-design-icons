<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon chart-areaspline-variant-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M22,21H2V3H4V15.54L9.5,6L16,9.78L20.24,2.45L21.97,3.45L22,21Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ChartAreasplineVariantIcon",
  props: {
    title: {
      type: String,
      default: "Chart Areaspline Variant icon"
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
