<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon cloud-alert-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M19 20H6C2.7 20 0 17.3 0 14C0 10.9 2.3 8.4 5.3 8C6.6 5.6 9.1 4 12 4C15.6 4 18.7 6.6 19.4 10C22 10.2 24 12.3 24 15C24 17.7 21.7 20 19 20M11 15V17H13V15H11M11 13H13V7H11V13Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "CloudAlertIcon",
  props: {
    title: {
      type: String,
      default: "Cloud Alert icon"
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
