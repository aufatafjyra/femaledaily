<template>
  <div class="article-card">
    <div class="card">
        <img alt="Image" src="../assets/image.jpeg">
        <div class="card-body">
            <h5 style="color: black">Title</h5>
            <p><b style="color: grey">Username</b> <c style="color: #CBCBCB"> | 1 hour ago</c></p>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'ArticleCard'
}
</script>

<style>
.article-card .card {
    width: 21rem;
    margin-top: 20px;
    margin-bottom: 10px;
    border: none;
}

.article-card img {
    height: 10rem;
}
</style>