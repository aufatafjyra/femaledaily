<template>
  <div class="match-product">
      <div class="section-one">
          <img alt="Image" src="../assets/image.png">
          <div class="match-text-content">
              <h3>Looking for products that are just simply perfect for you?</h3>
              <h5>Here are some products that we believe match your skin, hair, and body! Have we mentioned that they solve your concerns too?</h5>
              <button type="button" class="btn" style="background-color: #C93B51; color: white">See My Matches</button>
          </div>
      </div>

      <div class="section-two">
          <EditorCards />
          <EditorCards />
          <EditorCards />
      </div>
  </div>
</template>

<script>
import EditorCards from '@/components/EditorCards.vue'

export default {
    name: 'MatchProduct',
    components: {
        EditorCards
    }
}
</script>

<style>
.match-product {
    display: grid;
    grid-template-columns: 0.8fr 1fr;
    background-color: #F7DBE0;
    margin-top: 70px;
    margin-bottom: 70px;
    padding: 20px;
}

.section-one {
    display: grid;
    grid-template-columns: 0.8fr 1fr;
}

.section-two {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    padding-right: 110px;
}

.section-one h6 {
    margin-top: 20px;
}

.section-one .btn {
    margin-top: 20px;
}
</style>