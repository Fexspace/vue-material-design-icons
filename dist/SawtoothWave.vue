<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon sawtooth-wave-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M11 22V6.83L2 16V13.17L13 2V17.17L22 8V10.83L11 22Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SawtoothWaveIcon",
  props: {
    title: {
      type: String,
      default: "Sawtooth Wave icon"
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
