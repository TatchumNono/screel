<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="flex justify-center items-center h-screen">
    <Button text="Button" color="primary" />
  </div>
</template>

<script>
// import LocalLang from "@/components/LocalLang.vue";
import Button from "@/components/modules/buttons/button.vue";
export default {
  components: {
    Button,
  },
};
</script>
