<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon math-norm-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M14 21V3H16V21H14M8 21V3H10V21H8Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "MathNormIcon",
  props: {
    title: {
      type: String,
      default: "Math Norm icon"
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
