<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon garage-open-variant-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M22 9V20H20V11H4V20H2V9L12 5L22 9M19 12H5V14H19V12Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "GarageOpenVariantIcon",
  props: {
    title: {
      type: String,
      default: "Garage Open Variant icon"
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
