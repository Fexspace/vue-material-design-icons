<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon music-rest-half-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M6 14H8V10H16V14H18V15H6V14Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "MusicRestHalfIcon",
  props: {
    title: {
      type: String,
      default: "Music Rest Half icon"
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
