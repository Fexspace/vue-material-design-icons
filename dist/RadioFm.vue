<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon radio-fm-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M3,7V17H5V13H8V11H5V9H9V7H3M13,7A2,2 0 0,0 11,9V17H13V9H15V16H17V9H19V17H21V9A2,2 0 0,0 19,7H13Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "RadioFmIcon",
  props: {
    title: {
      type: String,
      default: "Radio Fm icon"
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
