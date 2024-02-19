<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="bg-red text-white">
      <q-toolbar>
        
        <q-toolbar-title class="text-weight-bolder text-h5">
          Edex Tech
        </q-toolbar-title>

        <div class="gt-sm">
          <q-tabs class="text-weight-bolder text-h5">
            <q-tab name="Curriculum" label="Curriculum" />
            <q-tab name="Placement" label="Placement" />
            <q-tab name="Mentor" label="Mentor" />
            <q-tab name="Review" label="Review" />
            <q-tab name="FAQ" label="FAQ" />
          </q-tabs>
        </div>

        <q-btn 
          class="lt-md"
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="toggleLeftDrawer"
        />

      </q-toolbar>
    </q-header>
    <q-drawer
        v-model="leftDrawerOpen"
        bordered
      >
        <q-list>
          <q-item-label
            header
          >
            Edex Tech
          </q-item-label>

          <EssentialLink
            v-for="link in essentialLinks"
            :key="link.title"
            v-bind="link"
          />
        </q-list>
      </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
    <q-footer elevated>
      <div class="q-pa-sm text-center text-h5 bg-pink-3 gt-sm">
        Need Help? Talk to us at 01205096020 or Request Callback
      </div>
    </q-footer>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'
import EssentialLink from 'components/EssentialLink.vue'

const linksList = [
  {
    title: 'Curriculum',
    link: 'https://quasar.dev'
  },
  {
    title: 'Placement',
    link: 'https://github.com/quasarframework'
  },
  {
    title: 'Mentor',
    link: 'https://chat.quasar.dev'
  },
  {
    title: 'Review',
    link: 'https://forum.quasar.dev'
  },
  {
    title: 'FAQ',
    link: 'https://twitter.quasar.dev'
  }
]

export default defineComponent({
  name: 'MainLayout',

  components: {
    EssentialLink
  },

  setup () {
    const leftDrawerOpen = ref(false)

    return {
      essentialLinks: linksList,
      leftDrawerOpen,
      toggleLeftDrawer () {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  }
})
</script>
