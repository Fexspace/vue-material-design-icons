<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon size-xl-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M6 7H8L9 9.5L10 7H12L10 12L12 17H10L9 14.5L8 17H6L8 12L6 7M13 7H15V15H19V17H13V7Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SizeXlIcon",
  props: {
    title: {
      type: String,
      default: "Size Xl icon"
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
