<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon cellphone-dock-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M16,15H8V5H16M16,1H8C6.89,1 6,1.89 6,3V17A2,2 0 0,0 8,19H16A2,2 0 0,0 18,17V3C18,1.89 17.1,1 16,1M8,23H16V21H8V23Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "CellphoneDockIcon",
  props: {
    title: {
      type: String,
      default: "Cellphone Dock icon"
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
