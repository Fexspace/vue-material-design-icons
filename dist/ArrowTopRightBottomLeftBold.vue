<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon arrow-top-right-bottom-left-bold-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M18.17,8.66L21,11.5V3H12.5L15.34,5.83L5.83,15.34L3,12.5V21H11.5L8.66,18.17L18.17,8.66Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ArrowTopRightBottomLeftBoldIcon",
  props: {
    title: {
      type: String,
      default: "Arrow Top Right Bottom Left Bold icon"
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
