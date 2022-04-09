<template>
  <div class="home">
    <NavBar />
    <MenuBar />

    <div class="container">
      <div class="ads-section">
        <TopFrame />
        <BillboardFrame />
      </div>

      <div class="home-section">
        <EditorChoice />
      </div>
    </div>
    
    <div class="match-section">
      <MatchProduct />
    </div>

    <div class="container">
      <div class="ads-section">
        <BillboardFrame />
      </div>
    </div>

    <div class="container">
      <div class="home-section">
        <ArticleSection />
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar.vue'
import MenuBar from '@/components/MenuBar.vue'
import TopFrame from '@/components/TopFrame.vue'
import BillboardFrame from '@/components/BillboardFrame.vue'
import EditorChoice from '@/components/EditorChoice.vue'
import MatchProduct from '@/components/MatchProduct.vue'
import ArticleSection from '@/components/ArticleSection.vue'

export default {
  name: 'HomeView',
  components: {
    NavBar,
    MenuBar,
    TopFrame,
    BillboardFrame,
    EditorChoice,
    MatchProduct,
    ArticleSection
  }
}
</script>

<style scoped>
.ads-section {
  padding-right: 40px;
  padding-left: 40px;
}
</style>