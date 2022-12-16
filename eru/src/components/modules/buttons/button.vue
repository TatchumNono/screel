<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <button
    :class="computedClass"
    class="width-150px h-10 rounded-17px font-bold text-sm leading-5"
  >
    {{ text }}
  </button>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      default: "Press",
    },
    color: {
      type: String,
      default: "primary",
    },
  },
  computed: {
    computedClass() {
      let className = "";
      let col = "primary";

      console.log(col);

      // More complicated logic to determine what
      // class should be applied
      col === "primary"
        ? (className = "bg-blue-light hover:bg-blue-accent text-white")
        : (className = "bg-sky-grayLightMode-100 hover:bg-grayLightMode-200");

      return className;
    },
  },
};
</script>

<style scoped>
.width-150px {
  width: 150px;
}
.rounded-17px {
  border-radius: 17px;
}
</style>
