<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon axis-z-arrow-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12,2L16,6H13V13.82L22.39,19.25L21.39,21L12,15.56L2.61,21L1.61,19.25L11,13.82V6H8L12,2Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "AxisZArrowIcon",
  props: {
    title: {
      type: String,
      default: "Axis Z Arrow icon"
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
