<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon plus-thick-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M20 14H14V20H10V14H4V10H10V4H14V10H20V14Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "PlusThickIcon",
  props: {
    title: {
      type: String,
      default: "Plus Thick icon"
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
