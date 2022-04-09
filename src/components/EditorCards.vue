<template>
  <div class="editor-card">
      <div class="card">
        <img alt="Image" src="../assets/image.png">
        <div class="card-body">
            <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'EditorCards'
}
</script>

<style>
.editor-card .card {
    width: 13rem
}

.editor-card img {
    height: 12rem;
}

.editor-card .card-body {
    height: 10rem;
}
</style>