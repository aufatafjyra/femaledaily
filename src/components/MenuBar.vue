<template>
    <nav class="navbar navbar-expand-sm navbar-light bg-light" data-toggle="affix" style="background-color: white !important;">
        <div class="mx-auto d-sm-flex d-block flex-sm-nowrap">
            <div class="collapse navbar-collapse text-center" id="navbarsExample11">
                <ul class="navbar-nav">
                    <li class="nav-item">
                        <a class="nav-link" href="#">SKINCARE</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">MAKE UP</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">BODY</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">HAIR</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">FRAGRANCE</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">NAILS</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">TOOLS</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">BRANDS</a>
                    </li>
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
.abs-center-x {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
}

.nav-link {
    color: black !important;
}

.navbar {
    /* border-top: 1px solid #E3E3E3; */
    border-bottom: 1px solid #E3E3E3;
}
</style>