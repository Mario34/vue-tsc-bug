<template>
  <ElForm ref="formRef">
    <ElFormItem>
      <ElInput v-model="inputValue" />
    </ElFormItem>
  </ElForm>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import { ElForm, ElFormItem, ElInput } from 'element-plus'
// import { } from '@vue/shared'
import type { FormInstance } from 'element-plus'
const formRef = ref<FormInstance>()
const inputValue = ref('')
defineExpose({
  formRef,
})
</script>
