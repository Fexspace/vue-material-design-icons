<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon pi-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M4,5V7H6V19H8V7H14V16A3,3 0 0,0 17,19A3,3 0 0,0 20,16H18A1,1 0 0,1 17,17A1,1 0 0,1 16,16V7H18V5">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "PiIcon",
  props: {
    title: {
      type: String,
      default: "Pi icon"
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
