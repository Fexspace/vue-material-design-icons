<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon format-header6-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M3,4H5V10H9V4H11V18H9V12H5V18H3V4M15,4H19A2,2 0 0,1 21,6V7H19V6H15V10H19A2,2 0 0,1 21,12V16A2,2 0 0,1 19,18H15A2,2 0 0,1 13,16V6A2,2 0 0,1 15,4M15,12V16H19V12H15Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FormatHeader6Icon",
  props: {
    title: {
      type: String,
      default: "Format Header6 icon"
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
