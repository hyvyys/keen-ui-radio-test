<template>
  <div id="app">
    <UiRadioGroup
      name="radio-1"
      v-model="value"
      :options="options"
    />
  </div>
</template>

<script>
import UiRadioGroup from "keen-ui/src/UiRadioGroup.vue";

export default {
  name: 'app',
  components: {
    UiRadioGroup
  },
  data() {
    return {
      value: "",
      options: [
        { value: "", label: "default" },
        { value: "a", label: "option a" },
        { value: "v", label: "option b" },
      ],
    };
  }
}
</script>
