<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon hospital-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M18 14H14V18H10V14H6V10H10V6H14V10H18">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "HospitalIcon",
  props: {
    title: {
      type: String,
      default: "Hospital icon"
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
