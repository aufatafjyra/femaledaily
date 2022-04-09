<template>
  <div class="article">
      <h5>Latest Article</h5>
      <div class="article-desc">
        <h6>So you can make better purchase decision</h6>
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
</template>

<script>
import ArticleCard from '@/components/ArticleCard.vue'

export default {
    name: 'ArticleSection',
    components: {
        ArticleCard
    }
}
</script>

<style>
.article {
    margin-top: 70px;
}

.article h6 {
    color: #ACACAC;
}

.article-desc {
    display: grid;
    grid-template-columns: 1fr 1fr;
}

.article-section-content {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
}
</style>