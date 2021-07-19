<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon view-parallel-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M19 3V21H15V3H19M14 3V21H10V3H14M9 3V21H5V3H9Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ViewParallelIcon",
  props: {
    title: {
      type: String,
      default: "View Parallel icon"
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
