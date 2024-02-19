<template>
    <div class="q-pa-md">
      <div class="q-gutter-y-md">
        <q-option-group
          class="text-h5 q-px-xl text-center q-pb-md"
          v-model="panel"
          inline
          :options="[
            { label: 'Beginner', value: 'Beginner' },
            { label: 'Intermediate', value: 'Intermediate' },
            { label: 'Advanced', value: 'Advanced' }
          ]"
        />
  
        <q-tab-panels v-model="panel" animated class="shadow-2 rounded-borders">
          <q-tab-panel name="Beginner">
            <div class="text-h6">11.5 Months</div>
            <VerticalTab></VerticalTab>
          </q-tab-panel>
  
          <q-tab-panel name="Intermediate">
            <div class="text-h6">11.5 Months</div>
            <VerticalTab></VerticalTab>
          </q-tab-panel>
  
          <q-tab-panel name="Advanced">
            <div class="text-h6">9.5 Months</div>
            <VerticalTab></VerticalTab>
          </q-tab-panel>
        </q-tab-panels>
      </div>
    </div>
  </template>
  
  <script>
  import { ref } from 'vue'
  import VerticalTab from './VerticalTab.vue'
  
  export default { 
    name:'TabPanel',
    components:{VerticalTab},
    setup () {
      return {
        panel: ref('Beginner')
      }
    }
  }
  </script>
  