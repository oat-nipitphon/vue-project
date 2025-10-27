<template>
  <div>
    <input :class="`w-full ${props.class}`" :type="props.type" :placeholder="props.placeholder"
      :value="props.modelValue" @input="emit('update:modelValue', $event.target.value)" />
  </div>
</template>
<script setup>
const props = defineProps({
  class: {
    type: [String, Number],
    default: 'border rounded-md px-3 py-2 bg-white',
  },
  type: {
    type: String,
    default: 'text',
  },
  placeholder: {
    type: [String, Number],
    default: 'input request...',
  },
  modelValue: {
    type: [String, Number],
    default: null,
  },
});
const emit = defineEmits(["update:modelValue"]);
</script>
