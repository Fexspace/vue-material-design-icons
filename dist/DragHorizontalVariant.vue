<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon drag-horizontal-variant-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M21 11H3V9H21V11M21 13H3V15H21V13Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "DragHorizontalVariantIcon",
  props: {
    title: {
      type: String,
      default: "Drag Horizontal Variant icon"
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
