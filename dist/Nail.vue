<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon nail-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M13.5,5V16L12,22L10.5,16V5H13.5M17,2H7V4H17V2Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "NailIcon",
  props: {
    title: {
      type: String,
      default: "Nail icon"
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
