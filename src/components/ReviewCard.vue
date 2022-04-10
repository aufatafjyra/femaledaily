<template>
  <div class="review">
      <div class="card mt-3">
        <div class="card-body">
          <div class="card-title">
            <div class="card-image">
              <img alt="Image" src="../assets/image.jpeg">
            </div>
            <div>
              <h6 class="card-title">TITLE</h6>
              <h6 class="card-subtitle mb-2">subtitle</h6>
            </div>
          </div>
          <hr>
          <div class="card-details">
            <div class="card-rate">
              <img src="https://img.icons8.com/plumpy/30/000000/star--v1.png"/>
              <img src="https://img.icons8.com/plumpy/30/000000/star--v1.png"/>
              <img src="https://img.icons8.com/plumpy/30/000000/star--v1.png"/>
              <img src="https://img.icons8.com/plumpy/30/000000/star--v1.png"/>
              <img src="https://img.icons8.com/plumpy/30/000000/star--v1.png"/>
            </div>
            <p style="color: grey; font-size: 12px">2 hours ago</p>
          </div>
          <p class="card-text mt-2" style="font-size: 14px">Some quick example text to build on the card title and make up the bulk of the card's content. <a href="#" class="card-link">Read More</a> </p>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'ReviewCard'
}
</script>

<style>
.review .card {
  width: 19rem;
}

.review .card-title {
  display: grid;
  grid-template-columns: 0.3fr 1fr;
  grid-gap: 10px;
}

.review .card-title img {
  width: 4rem;
  height: 4rem;
}

.review .card-details {
  display: grid;
  grid-template-columns: 1fr 0.6fr;

}
</style>