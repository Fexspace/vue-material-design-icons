<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon bottle-tonic-plus-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M13 4H11L10 2H14L13 4M14 8V6H15V5H9V6H10V8C7.24 8 5 10.24 5 13V22H19V13C19 10.24 16.76 8 14 8M16 17H13V20H11V17H8V15H11V12H13V15H16V17Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "BottleTonicPlusIcon",
  props: {
    title: {
      type: String,
      default: "Bottle Tonic Plus icon"
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
