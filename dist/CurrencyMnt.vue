<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon currency-mnt-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M13 5V8.62L17 7.17V9.29L13 10.74V12.5L17 11.07V13.2L13 14.65V21H11V15.38L7 16.84V14.71L11 13.24V11.47L7 12.92V10.8L11 9.35V5H5V3H19V5H13Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "CurrencyMntIcon",
  props: {
    title: {
      type: String,
      default: "Currency Mnt icon"
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
