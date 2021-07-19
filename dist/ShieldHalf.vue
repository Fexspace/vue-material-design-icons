<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon shield-half-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12 1L3 5V11C3 16.5 6.8 21.7 12 23V1Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "ShieldHalfIcon",
  props: {
    title: {
      type: String,
      default: "Shield Half icon"
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
