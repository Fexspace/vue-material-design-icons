<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon message-arrow-left-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M20 2H4C2.9 2 2 2.9 2 4V22L6 18H20C21.1 18 22 17.1 22 16V4C22 2.9 21.1 2 20 2M16 11H11.5L13.3 12.8L12 14L8 10L12 6L13.2 7.2L11.5 9H16V11Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "MessageArrowLeftIcon",
  props: {
    title: {
      type: String,
      default: "Message Arrow Left icon"
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
