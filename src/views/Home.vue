
<script lang="ts" setup>
  import HelloWorld from '@/components/HelloWorld.vue'

  const clicked = async() => {
    window.alert('test')

    const temp = localStorage.getItem('test')
    console.error(`temp : ${temp}`)
    localStorage.setItem('test', 'test')
  }
</script>


<template>
  <v-card hover>
    <v-card-title>Test</v-card-title>
    <v-card-text>Contents #1
      Contents #2
      Contents #3
    </v-card-text>
    <v-card-actions>
      <v-btn @click="clicked">Click</v-btn>
    </v-card-actions>
  </v-card>
  <HelloWorld />
</template>
