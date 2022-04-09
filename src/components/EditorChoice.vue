<template>
  <div class="editor">
      <h5>Editor's Choice</h5>
      <h6>Curated with love</h6>
      <div class="card-section">
          <EditorCard />
          <EditorCard />
          <EditorCard />
          <EditorCard />
          <EditorCard />
      </div>
  </div>
</template>

<script>
import EditorCard from '@/components/EditorCards.vue'

export default {
    name: 'EditorChoice',
    components: {
        EditorCard
    }
}
</script>

<style>
.editor {
    margin-top: 40px;
}

.editor h6 {
    color: #ACACAC;
}

.editor .card-section {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
    grid-gap: 20px
}
</style>