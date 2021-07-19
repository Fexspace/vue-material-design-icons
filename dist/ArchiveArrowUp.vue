<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon archive-arrow-up-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M4 21H20V8H4M14 15V18H10V15H7L12 10L17 15M3 3H21V7H3">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ArchiveArrowUpIcon",
  props: {
    title: {
      type: String,
      default: "Archive Arrow Up icon"
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
