<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon picture-in-picture-top-right-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M19,7H11V13H19V7M17,11H13V9H17V11M21,3H3A2,2 0 0,0 1,5V19C1,20.11 1.9,21 3,21H21A2,2 0 0,0 23,19V5C23,3.91 22.1,3 21,3M21,19H3V5H21V19Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "PictureInPictureTopRightOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Picture In Picture Top Right Outline icon"
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
