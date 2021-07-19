<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon exclamation-thick-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M10 3H14V14H10V3M10 21V17H14V21H10Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ExclamationThickIcon",
  props: {
    title: {
      type: String,
      default: "Exclamation Thick icon"
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
