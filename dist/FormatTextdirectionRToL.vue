<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon format-textdirection-r-to-l-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M8,17V14L4,18L8,22V19H20V17M10,10V15H12V4H14V15H16V4H18V2H10A4,4 0 0,0 6,6A4,4 0 0,0 10,10Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FormatTextdirectionRToLIcon",
  props: {
    title: {
      type: String,
      default: "Format Textdirection R To L icon"
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
