<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon align-vertical-bottom-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M11 18H5V2H11V18M19 8H13V18H19V8M22 20H2V22H22V20Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "AlignVerticalBottomIcon",
  props: {
    title: {
      type: String,
      default: "Align Vertical Bottom icon"
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
