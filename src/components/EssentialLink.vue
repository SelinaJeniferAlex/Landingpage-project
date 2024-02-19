<template>
  <div class="text-center">
    

  <q-item
    clickable
    tag="a"
    target="_self"
    :href="link"
  
  >
    <q-item-section>
      <q-btn>{{ title }}</q-btn>
    </q-item-section>
  </q-item>
  </div>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'EssentialLink',
  props: {
    title: {
      type: String,
      required: true
    },

    link: {
      type: String,
      default: '#'
    },
  }
})
</script>
