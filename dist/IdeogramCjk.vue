<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon ideogram-cjk-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M11 4V6H4V10H6V8H18V10H20V6H13V4M8 10V12H13.59L11.59 14H4V16H11V18H10V20H13V16H20V14H14.21L16 12.21V10Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "IdeogramCjkIcon",
  props: {
    title: {
      type: String,
      default: "Ideogram Cjk icon"
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
