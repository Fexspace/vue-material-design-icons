<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon loading-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12,4V2A10,10 0 0,0 2,12H4A8,8 0 0,1 12,4Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "LoadingIcon",
  props: {
    title: {
      type: String,
      default: "Loading icon"
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
