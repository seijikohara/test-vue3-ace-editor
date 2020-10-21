<template>
  <VAceEditor v-model="state.content" lang="html" theme="chrome" />
</template>

<script lang="ts">
import { defineComponent, reactive } from "vue";
import { VAceEditor } from "vue3-ace-editor";

export default defineComponent({
  name: "Editor",
  components: { VAceEditor },
  setup() {
    const state = reactive({
      content: "content text"
    });
    return {
      state
    };
  }
});
</script>
