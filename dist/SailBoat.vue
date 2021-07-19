<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon sail-boat-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M14,3L5,14H14M3,16L6,21H18L21,16">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SailBoatIcon",
  props: {
    title: {
      type: String,
      default: "Sail Boat icon"
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
