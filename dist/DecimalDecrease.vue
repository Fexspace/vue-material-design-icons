<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon decimal-decrease-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M12,17L15,20V18H21V16H15V14L12,17M9,5A3,3 0 0,1 12,8V11A3,3 0 0,1 9,14A3,3 0 0,1 6,11V8A3,3 0 0,1 9,5M9,7A1,1 0 0,0 8,8V11A1,1 0 0,0 9,12A1,1 0 0,0 10,11V8A1,1 0 0,0 9,7M4,12A1,1 0 0,1 5,13A1,1 0 0,1 4,14A1,1 0 0,1 3,13A1,1 0 0,1 4,12Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "DecimalDecreaseIcon",
  props: {
    title: {
      type: String,
      default: "Decimal Decrease icon"
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
