<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon bowl-outline-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M2 12V15C2 18.9 5.1 22 9 22H15C18.9 22 22 18.9 22 15V12H2M4 14H20V15C20 17.8 17.8 20 15 20H9C6.2 20 4 17.8 4 15V14Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "BowlOutlineIcon",
  props: {
    title: {
      type: String,
      default: "Bowl Outline icon"
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
