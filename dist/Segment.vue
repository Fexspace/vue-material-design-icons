<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon segment-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M21,8H3V6H21M9,13H21V11H9M9,18H21V16H9">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SegmentIcon",
  props: {
    title: {
      type: String,
      default: "Segment icon"
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
