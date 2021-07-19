<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon square-off-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M20.84 22.73L19.11 21H3V4.89L1.11 3L2.39 1.73L22.11 21.46L20.84 22.73M21 3H6.2L21 17.8V3Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SquareOffIcon",
  props: {
    title: {
      type: String,
      default: "Square Off icon"
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
