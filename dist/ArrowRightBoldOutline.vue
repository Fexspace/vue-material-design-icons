<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon arrow-right-bold-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M11,16H3V8H11V2L21,12L11,22V16M13,7V10H5V14H13V17L18,12L13,7Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ArrowRightBoldOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Arrow Right Bold Outline icon"
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
