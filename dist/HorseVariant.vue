<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon horse-variant-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M20 8V16L17 17L13.91 11.5C13.65 11.04 12.92 11.27 13 11.81L14 21L4 17L5.15 8.94C5.64 5.53 8.56 3 12 3H20L18.42 5.37C19.36 5.88 20 6.86 20 8Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "HorseVariantIcon",
  props: {
    title: {
      type: String,
      default: "Horse Variant icon"
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
