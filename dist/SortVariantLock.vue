<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon sort-variant-lock-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M3,13V11H15V13H3M3,6H21V8H3V6M3,18V16H9V18H3M22,22H14V18H15V17A3,3 0 0,1 18,14A3,3 0 0,1 21,17V18H22V22M18,16A1,1 0 0,0 17,17V18H19V17A1,1 0 0,0 18,16Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "SortVariantLockIcon",
  props: {
    title: {
      type: String,
      default: "Sort Variant Lock icon"
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
