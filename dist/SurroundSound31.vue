<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon surround-sound31-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M13,17A1,1 0 0,1 12,16A1,1 0 0,1 13,15A1,1 0 0,1 14,16A1,1 0 0,1 13,17M19,7V15H20V17H16V15H17V9H16L17,7H19M4,7H8A2,2 0 0,1 10,9V15A2,2 0 0,1 8,17H4V15H8V13H5V11H8V9H4V7Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SurroundSound31Icon",
  props: {
    title: {
      type: String,
      default: "Surround Sound31 icon"
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
