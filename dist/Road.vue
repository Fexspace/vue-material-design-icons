<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon road-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M11,16H13V20H11M11,10H13V14H11M11,4H13V8H11M4,22H20V2H4V22Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "RoadIcon",
  props: {
    title: {
      type: String,
      default: "Road icon"
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
