<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon square-medium-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M14,10V14H10V10H14M16,8H8V16H16V8Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SquareMediumOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Square Medium Outline icon"
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
