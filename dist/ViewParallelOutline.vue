<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon view-parallel-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M19 3H5V21H19V3M17 19H15V5H17V19M13 19H11V5H13V19M7 5H9V19H7V5Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ViewParallelOutlineIcon",
  props: {
    title: {
      type: String,
      default: "View Parallel Outline icon"
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
