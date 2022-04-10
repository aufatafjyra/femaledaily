<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light" style="background-color: white !important">
    <div class="container-fluid">
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <a class="navbar-brand" href="#">
        <img alt="Female Daily Logo" src="../assets/logo.png">
      </a>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <form class="d-flex col-md-10">
          <input class="form-control me-2" type="search" placeholder="Search products, articles, topics, brands, etc" aria-label="Search">
        </form>
      </div>
      <button type="button" class="btn btn-danger mt-0 mb-0">LOGIN / SIGNUP</button>
    </div>
  </nav>
</template>

<script>
export default {
    name: 'NavBar'
}
</script>

<style>
  img {
    height: 30px;
  }
</style>