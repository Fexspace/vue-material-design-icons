<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon cup-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M3 2L5 20.23C5.13 21.23 5.97 22 7 22H17C18 22 18.87 21.23 19 20.23L21 2H3M5.22 4H18.78L17 20H7L5.22 4Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "CupOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Cup Outline icon"
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
