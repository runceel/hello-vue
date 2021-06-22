<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  setup() {
    fetch('/.auth/me').then(x =>
    {
      return x.json();
    }).then(x => console.log(x));
  },
})
</script>
