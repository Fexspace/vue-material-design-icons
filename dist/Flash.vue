<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon flash-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M7,2V13H10V22L17,10H13L17,2H7Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "FlashIcon",
  props: {
    title: {
      type: String,
      default: "Flash icon"
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
