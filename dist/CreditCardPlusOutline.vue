<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon credit-card-plus-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M21,18H24V20H21V23H19V20H16V18H19V15H21V18M19,8V6H3V8H19M19,12H3V18H14V20H3C1.89,20 1,19.1 1,18V6C1,4.89 1.89,4 3,4H19A2,2 0 0,1 21,6V13H19V12Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "CreditCardPlusOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Credit Card Plus Outline icon"
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
