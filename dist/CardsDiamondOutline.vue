<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon cards-diamond-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12 2L5 12L12 22L19 12M7.44 12L12 5.5L16.56 12L12 18.5">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "CardsDiamondOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Cards Diamond Outline icon"
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
