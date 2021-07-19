<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon sort-reverse-variant-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M3 11H15V13H3M3 18V16H21V18M3 6H9V8H3Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SortReverseVariantIcon",
  props: {
    title: {
      type: String,
      default: "Sort Reverse Variant icon"
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
