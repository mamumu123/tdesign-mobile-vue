<template>
  <div>
    <t-fab :icon="iconFunc" text="按钮文字" :button-props="baseButtonProps" :style="customStyle" @click="onClick" />
  </div>
</template>

<script lang="ts" setup>
import { h } from 'vue';
import { AddIcon } from 'tdesign-icons-vue-next';

const iconFunc = () => h(AddIcon);
const baseButtonProps = {
  variant: 'outline',
};
const customStyle = 'right: 16px; bottom: 32px;';
const onClick = () => {
  console.log('click Fab');
};
</script>

<style lang="less" scoped></style>
