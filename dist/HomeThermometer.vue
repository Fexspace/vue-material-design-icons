<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon home-thermometer-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12 3L2 12H5V20H19V12H22L12 3M12 8A1 1 0 0 1 13 9V14.27A2 2 0 0 1 14 16A2 2 0 0 1 12 18A2 2 0 0 1 10 16A2 2 0 0 1 11 14.27V9A1 1 0 0 1 12 8Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "HomeThermometerIcon",
  props: {
    title: {
      type: String,
      default: "Home Thermometer icon"
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
