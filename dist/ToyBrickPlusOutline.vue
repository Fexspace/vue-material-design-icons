<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon toy-brick-plus-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M19 6V5A2 2 0 0 0 17 3H15A2 2 0 0 0 13 5V6H11V5A2 2 0 0 0 9 3H7A2 2 0 0 0 5 5V6H3V20H14V18H5V8H19V13H21V6M21 15V18H24V20H21V23H19V20H16V18H19V15Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ToyBrickPlusOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Toy Brick Plus Outline icon"
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
