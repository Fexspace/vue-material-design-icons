<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon chart-multiple-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M22 16V18H6V2H8V13.57L13.71 4.57L16.87 6.68L19.29 4.26L20.71 5.68L17.13 9.29L14.29 7.4L8.82 16M4 20V4H2V22H22V20Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ChartMultipleIcon",
  props: {
    title: {
      type: String,
      default: "Chart Multiple icon"
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
