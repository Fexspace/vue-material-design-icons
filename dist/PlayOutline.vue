<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon play-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M8.5,8.64L13.77,12L8.5,15.36V8.64M6.5,5V19L17.5,12">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "PlayOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Play Outline icon"
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
