<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon surround-sound71-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12,17A1,1 0 0,1 11,16A1,1 0 0,1 12,15A1,1 0 0,1 13,16A1,1 0 0,1 12,17M18,7V15H19V17H15V15H16V9H15L16,7H18M11,7L8,17H6L8.4,9H5V7H11Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SurroundSound71Icon",
  props: {
    title: {
      type: String,
      default: "Surround Sound71 icon"
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
