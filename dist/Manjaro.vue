<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon manjaro-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M2 2V22H7.6V7.6H14.8V2H2M9.2 9.2V22H14.8V9.2H9.2M16.4 2V22H22V2H16.4Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ManjaroIcon",
  props: {
    title: {
      type: String,
      default: "Manjaro icon"
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
