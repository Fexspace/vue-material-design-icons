<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon settings-helper-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M7,22H9V24H7V22M11,22H13V24H11V22M15,22H17V24H15V22Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SettingsHelperIcon",
  props: {
    title: {
      type: String,
      default: "Settings Helper icon"
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
