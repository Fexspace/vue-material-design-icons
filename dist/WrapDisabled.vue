<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon wrap-disabled-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M16,7H3V5H16V7M3,19H16V17H3V19M22,12L18,9V11H3V13H18V15L22,12Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "WrapDisabledIcon",
  props: {
    title: {
      type: String,
      default: "Wrap Disabled icon"
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
