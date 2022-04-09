<template>
  <nav class="navbar navbar-default">
    <div class="container text-center">
        <div id="navbar" class="navbar-collapse">
            <ul class="nav navbar-nav">
                <li><a href="#">SKINCARE</a></li>
                <li><a href="#">MAKE UP</a></li>
                <li><a href="#">BODY</a></li>
                <li><a href="#">HAIR</a></li>
                <li><a href="#">FRAGRANCE</a></li>
                <li><a href="#">NAILS</a></li>
                <li><a href="#">HAIR</a></li>
                <li><a href="#">BRANDS</a></li>
            </ul>
        </div>
    </div>
</nav>
</template>

<script>
export default {
    name: 'MenuBar'
}
</script>

<style>
.navbar .navbar-header,
.navbar-collapse {
    float:none;
    display:inline-block;
    vertical-align: top;
    padding-left: 0;
    padding-right: 0;
    background-color: white;
}

@media (max-width: 768px) {
    .navbar-collapse  {
        display: block;
    }
}
</style>