<template>
    <div class="popular-group">
        <div class="card shadow">
            <img alt="Image" src="../assets/image.jpeg" class="mt-5 rounded-circle"> 
            <div class="card-body">
                <h5 class="card-title">Embrace the curl</h5>
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
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
}
</style>