<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon axis-y-arrow-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M22.5,20.5L17,21.96L18.53,19.35L12,15.58L2.61,21L1.61,19.27L11,13.85V3H13V13.85L19.53,17.61L21,15.03L22.5,20.5Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "AxisYArrowIcon",
  props: {
    title: {
      type: String,
      default: "Axis Y Arrow icon"
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
