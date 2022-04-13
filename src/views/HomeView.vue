<template>
  <div class="home">
    <NavBar />
    <MenuBar />

    <div class="container">
      <div class="ads-section">
        <TopFrame />
        <BillboardFrame />
      </div>

      <div class="editor container">
        <h5>Editor's Choice</h5>
        <h6>Curated with love</h6>
        <div class="card-section">
            <div class="editor-card" v-for="products in product" v-bind:key="products.id">
                <div class="card">
                    <img alt="Image" v-bind:src="products.product['image']">
                    <div class="card-body">
                        <p class="card-text"><b>{{products.product['name']}}</b></p>
                        <p class="card-text">{{products.product['description']}}</p>
                    </div>
                </div>
            </div>
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
          <h6 style="color: #E50914" class="justify-content-end">See more</h6>
        </div>
        <div class="article-section-content">
            <div class="article-card" v-for="article in articles" v-bind:key="article.id">
                <div class="card">
                    <img alt="Image" v-bind:src="article.image">
                    <div class="card-body">
                        <h5 style="color: black">{{article.title}}</h5>
                        <p><b style="color: grey">{{article.author}}</b> <c style="color: #CBCBCB"> | 1 hour ago</c></p>
                    </div>
                </div>
            </div>
        </div>
      </div>

      <div class="review mb-5">
        <div class="review-content">
          <h5>Latest Reviews</h5>
          <div class="section-title">
            <h6 class="mb-4 mt-1">So you can make better purchase decision</h6>
            <h6 style="color: #E50914" class="justify-content-end">See more</h6>
          </div>
          <div class="section-card">
            <div class="review" v-for="review in reviews" v-bind:key="review.id">
                <div class="card mt-3">
                    <div class="card-body">
                    <div class="card-title">
                        <div class="card-image">
                        <img alt="Image" v-bind:src="review.product['image']">
                        </div>
                        <div>
                        <h6 class="card-title">{{review.product['name']}}</h6>
                        <h6 class="card-subtitle mb-2">{{review.product['desc']}}</h6>
                        </div>
                    </div>
                    <hr>
                    <div class="card-details">
                        <div class="card-rate">
                        </div>
                        <p style="color: grey; font-size: 12px">2 hours ago</p>
                    </div>
                    <p class="card-text mt-2" style="font-size: 14px">{{review.comment}}<a href="#" class="card-link">Read More</a> </p>
                    </div>
                </div>
            </div>
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
import Vue from 'vue';
import axios from 'axios';
import VueAxios from 'vue-axios'
import NavBar from '@/components/NavBar.vue'
import MenuBar from '@/components/MenuBar.vue'
import TopFrame from '@/components/TopFrame.vue'
import BillboardFrame from '@/components/BillboardFrame.vue'
import GroupCard from '@/components/PopularGroupCard.vue'
import BottomFooter from '@/components/BottomFooter.vue' 

Vue.use(VueAxios,axios)

export default {
  name: 'HomeView',
  data (){
    return{
     dialog: false,
      drawer: null,
      items: [{ icon: 'dashboard', text: 'Dashboard', route :'/' },{ icon: 'person', text: 'User', route:'/User' }],
      product: [],
      articles:[],
      reviews:[]
    }
  },
  mounted() {
      axios
        .get('https://virtserver.swaggerhub.com/hqms/FDN-WP/0.1/wp')
        .then(response => {
            this.product = response.data["editor's choice"];
            this.articles = response.data["latest articles"];
            this.reviews = response.data["latest review"];
        })
        .catch(error => {
            console.log(error)
        })
  },
  components: {
    NavBar,
    MenuBar,
    TopFrame,
    BillboardFrame,
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
    display: grid !important;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr !important;
    grid-gap: 20px;
    column-count: 5;
}

.editor-card img {
    height: 12rem;
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
    column-count: 3;
}

.article-card .card {
    width: 21rem;
    margin-top: 20px;
    margin-bottom: 10px;
    border: none;
}

.article-card img {
    height: 10rem;
}

.review {
  display: grid;
  grid-template-columns: 1fr 0.3fr;
  grid-gap: 50px;
  column-count: 2;
}

.review img {
  width: 300px;
  height: 250px;
}

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