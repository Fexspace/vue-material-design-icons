<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon arrow-up-down-bold-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M10,8H6L12,2L18,8H14V16H18L12,22L6,16H10V8Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ArrowUpDownBoldIcon",
  props: {
    title: {
      type: String,
      default: "Arrow Up Down Bold icon"
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
