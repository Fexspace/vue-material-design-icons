<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon music-rest-whole-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M18 10H16V14H8V10H6V9H18V10Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "MusicRestWholeIcon",
  props: {
    title: {
      type: String,
      default: "Music Rest Whole icon"
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
