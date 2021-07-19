<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon drag-vertical-variant-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M11 21H9V3H11V21M15 3H13V21H15V3Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "DragVerticalVariantIcon",
  props: {
    title: {
      type: String,
      default: "Drag Vertical Variant icon"
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
