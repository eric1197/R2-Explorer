<template>
  <q-btn dense flat round icon="menu" @click="$emit('toggle')" />

  <q-toolbar-title style="overflow: unset" class="text-bold">
    <q-avatar>
      <img src="/logo.png">
    </q-avatar>
    Tings-Drive
  </q-toolbar-title>
  <q-space />
  <div>
    <bucket-picker/>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import BucketPicker from "components/main/BucketPicker.vue";

export default defineComponent({
  name: "TopBar",
  emits: ['toggle'],
  components: { BucketPicker }
});
</script>
