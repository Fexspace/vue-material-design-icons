<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon surround-sound21-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M4 7V9H8V11H6A2 2 0 0 0 4 13V17H10V15H6V13H8A2 2 0 0 0 10 11V9A2 2 0 0 0 8 7H4M16 7V9H18V17H20V7H16M12 15V17H14V15H12Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SurroundSound21Icon",
  props: {
    title: {
      type: String,
      default: "Surround Sound21 icon"
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
