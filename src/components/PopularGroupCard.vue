<template>
    <div class="popular-group">
        <div class="card shadow">
            <img alt="Image" src="../assets/curl.png" class="mt-5 rounded-circle"> 
            <div class="card-body">
                <h5 class="card-title">Embrace the curl</h5>
                <p class="card-text">May our curls pop and never stop!</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'GroupCard'
}
</script>

<style>
.popular-group .card {
    width: 16rem;
    text-align: center;
}

.popular-group img {
    width: 10rem;
    height: 10rem;
    margin: 0 auto;
}
</style>