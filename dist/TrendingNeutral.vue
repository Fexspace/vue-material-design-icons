<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon trending-neutral-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M22,12L18,8V11H3V13H18V16L22,12Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "TrendingNeutralIcon",
  props: {
    title: {
      type: String,
      default: "Trending Neutral icon"
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
