<template>
  <span :aria-hidden="decorative"
        :aria-label="title"
        class="material-design-icon microsoft-azure-devops-icon"
        role="img">
    <svg :fill="fillColor"
         class="material-design-icon__svg"
         :width="size"
         :height="size"
         viewBox="0 0 24 24">
      <path d="M22 18L17 22L9 19V22L4.81 16.25L17.72 17.3V6.34L22 5.65V18M4.81 16.25V8.96L17.72 6.34L10.6 2V4.84L3.97 6.76L2 9.38V15.07L4.81 16.25Z">
        <title>{{ title }}</title>
      </path>
    </svg>
  </span>
</template>

<script>
export default {
  name: "MicrosoftAzureDevopsIcon",
  props: {
    title: {
      type: String,
      default: "Microsoft Azure Devops icon"
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
