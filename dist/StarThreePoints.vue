<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon star-three-points-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12,2.6L9,12.4L2,19.9L12,17.6L22,20L15,12.5L12,2.6Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "StarThreePointsIcon",
  props: {
    title: {
      type: String,
      default: "Star Three Points icon"
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
