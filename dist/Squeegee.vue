<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon squeegee-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M22,2V5H2V2H22M2,8H7L9,10H10V20A2,2 0 0,0 12,22A2,2 0 0,0 14,20V10H15L17,8H22V6H2V8Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SqueegeeIcon",
  props: {
    title: {
      type: String,
      default: "Squeegee icon"
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
