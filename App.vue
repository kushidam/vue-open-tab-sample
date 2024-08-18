<script setup>
import { ref } from 'vue'

const msg = ref('Hello World!')
const q1 = ref('param1')
const q2 = ref('param2')

const openNewTab = () => {
  // q1とq2の値を取得してクエリパラメータとして追加
  const url = `/open-tab?q1=${encodeURIComponent(q1.value)}&q2=${encodeURIComponent(q2.value)}`;
  window.open(url, '_blank');
}
</script>

<template>
  <h1>{{ msg }}</h1>
  <input v-model="msg" />
  <div>
    <h2>URL Params</h2>
    <input v-model="q1" />
    <input v-model="q2" />
  </div>
  <button @click="openNewTab">Open New Tab</button>
</template>
