<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon file-swap-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M14 2H6A2 2 0 0 0 4 4V20A2 2 0 0 0 6 22H18A2 2 0 0 0 20 20V8M14 18V16H10V18L7 15L10 12V14H14V12L17 15M13 9V3.5L18.5 9Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FileSwapIcon",
  props: {
    title: {
      type: String,
      default: "File Swap icon"
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
