<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon axis-x-arrow-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M1.5,20.5L3,15.03L4.46,17.6L11,13.82V3H13V13.82L22.39,19.25L21.39,21L12,15.56L5.46,19.33L7,21.96L1.5,20.5Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "AxisXArrowIcon",
  props: {
    title: {
      type: String,
      default: "Axis X Arrow icon"
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
