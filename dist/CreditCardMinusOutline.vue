<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon credit-card-minus-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M24 18V20H16V18M19 8V6H3V8H19M19 12H3V18H14V20H3C1.89 20 1 19.1 1 18V6C1 4.89 1.89 4 3 4H19C20.11 4 21 4.89 21 6V13H19V12Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "CreditCardMinusOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Credit Card Minus Outline icon"
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
