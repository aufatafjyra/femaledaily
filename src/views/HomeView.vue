<template>
  <div class="home">
    <NavBar />
    <MenuBar />

    <div class="container">
      <div class="ads-section">
        <TopFrame />
        <BillboardFrame />
      </div>

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
    </div>
    
    <div class="match-product">
      <div class="section-one">
          <img alt="Image" src="../assets/image.jpeg">
          <div class="match-text-content">
              <h3>Looking for products that are just simply perfect for you?</h3>
              <h5>Here are some products that we believe match your skin, hair, and body! Have we mentioned that they solve your concerns too?</h5>
              <button type="button" class="btn" style="background-color: #C93B51; color: white">See My Matches</button>
          </div>
      </div>

      <div class="section-two">
          <EditorCard />
          <EditorCard />
          <EditorCard />
      </div>
  </div>

    <div class="container">
      <div class="ads-section">
        <BillboardFrame />
      </div>
    </div>

    <div class="container">
      <div class="section-content mt-5">
        <h5>Latest Article</h5>
        <div class="section-title">
          <h6 class="mb-4 mt-1">So you can make better purchase decision</h6>
          <h6 style="color: #E50914">See more</h6>
        </div>
        <div class="article-section-content">
            <ArticleCard />
            <ArticleCard />
            <ArticleCard />
            <ArticleCard />
            <ArticleCard />
            <ArticleCard />
        </div>
      </div>

      <div class="review mb-5">
        <div class="review-content">
          <h5>Latest Reviews</h5>
          <div class="section-title">
            <h6 class="mb-4 mt-1">So you can make better purchase decision</h6>
            <h6 style="color: #E50914">See more</h6>
          </div>
          <div class="section-card">
            <ReviewCard />
            <ReviewCard />
          </div>
        </div>
        <img alt="Image" src="../assets/image.jpeg" class="mt-5"> 
      </div>

      <div class="group-content mb-5">
        <h5>Popular Groups</h5>
        <div class="section-title">
          <h6 class="mb-4 mt-1">Where the beauty TALK are</h6>
          <h6 style="color: #E50914" class="justify-content-end">See more</h6>
        </div>
        <div class="section-card">
          <GroupCard />
          <GroupCard />
          <GroupCard />
          <GroupCard />
        </div>
      </div>

      <div class="section-content mb-5">
        <h5>Latest Videos</h5>
        <div class="section-title">
          <h6 class="mb-4 mt-1">Watch and learn, ladies</h6>
          <h6 style="color: #E50914" class="justify-content-end">See more</h6>
        </div>
        <div class="section-video" style="height: 25rem">
          <div class="section-one">
            <img alt="Image" src="../assets/image.jpeg" style="width: 100%; height: 25rem">
          </div>
          <div class="section-two">
            <img alt="Image" src="../assets/image.jpeg" style="width: 100%; height: 12rem">
            <img alt="Image" src="../assets/image.jpeg" style="width: 100%; height: 12rem">
          </div>
        </div>
      </div>

      <div class="section-content mb-5">
        <h5>Top Brands</h5>
        <div class="section-title">
          <h6 class="mb-4 mt-1">We all know and love</h6>
          <h6 style="color: #E50914" class="justify-content-end">See more</h6>
        </div>
        <div class="brand-section">
          <img alt="Image" src="../assets/image.jpeg" style="width: 100%; height: 7rem">
          <img alt="Image" src="../assets/image.jpeg" style="width: 100%; height: 7rem">
          <img alt="Image" src="../assets/image.jpeg" style="width: 100%; height: 7rem">
          <img alt="Image" src="../assets/image.jpeg" style="width: 100%; height: 7rem">
          <img alt="Image" src="../assets/image.jpeg" style="width: 100%; height: 7rem">
          <img alt="Image" src="../assets/image.jpeg" style="width: 100%; height: 7rem">
        </div>
        <h5 class="mt-5">Female Daily - Find everything you want to know about beauty on Female Daily</h5>
        <h6 class="mb-1 mt-2" style="color: black">Product Reviews, Tips & Tricks, Expert and Consumer Opinions, Beauty Tutorials, Discussions, Beauty Workshops, anything!</h6>
        <h6 class="mb-4" style="color: black">We are here to be your friendly solution to all things beauty, inside and out!</h6>
      </div>
    </div>
    <hr>
    <div class="ads-section">
      <BottomFooter />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar.vue'
import MenuBar from '@/components/MenuBar.vue'
import TopFrame from '@/components/TopFrame.vue'
import BillboardFrame from '@/components/BillboardFrame.vue'
import EditorCard from '@/components/EditorCards.vue'
import ArticleCard from '@/components/ArticleCard.vue'
import ReviewCard from '@/components/ReviewCard.vue'
import GroupCard from '@/components/PopularGroupCard.vue'
import BottomFooter from '@/components/BottomFooter.vue'

export default {
  name: 'HomeView',
  components: {
    NavBar,
    MenuBar,
    TopFrame,
    BillboardFrame,
    EditorCard,
    ArticleCard,
    ReviewCard,
    GroupCard,
    BottomFooter
    
  }
}
</script>

<style scoped>
.ads-section {
  padding-right: 40px;
  padding-left: 40px;
}

.editor {
    margin-top: 40px;
}

h6 {
    color: #ACACAC;
}

.editor .card-section {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
    grid-gap: 20px
}

.match-product {
    display: grid;
    grid-template-columns: 0.8fr 1fr;
    background-color: #F7DBE0;
    margin-top: 70px;
    margin-bottom: 70px;
    padding: 20px;
}

.match-product .section-one {
    display: grid;
    grid-template-columns: 0.8fr 1fr;
}

.match-product .section-two {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    padding-right: 110px;
}

.match-product img {
  width: 17rem;
  height: 100%;
}

.match-product .section-one h6 {
    margin-top: 20px;
}

.match-product .section-one .btn {
    margin-top: 20px;
}

.section-title {
    display: grid;
    grid-template-columns: 1fr 1fr;
}

.section-card {
  display: grid;
  grid-template-columns: 1fr 1fr;
}

.article-section-content {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
}

.review {
  display: grid;
  grid-template-columns: 1fr 0.3fr;
  grid-gap: 50px;
}

.review img {
  width: 300px;
  height: 250px;
}

.group-content .section-card{
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
}

.section-video {
  display: grid;
  grid-template-columns: 1fr 0.5fr;
  grid-gap: 35px;
}

.section-video .section-two {
  display: grid;
  grid-template-rows: 1fr 1fr;
  grid-gap: 20px;
}

.brand-section {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;
  grid-gap: 20px;
}
</style>