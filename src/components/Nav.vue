<template>
    <nav>
        <div class="logo">
            Mild
        </div>
        <div class="nav-items">
            <a href="#">home</a>
            <a href="#">About</a>
            <a href="#">Contents</a>
        </div>
    </nav>
</template>
<script>
export default {
    name:"Nav"
}
</script>
<style>
nav{
    display:flex;
    justify-content: space-between;
    background: rgb(250, 236, 208);
    padding: 20px;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 1;
    position: fixed;

}
.logo{
    color: rgb(97, 139, 34);
    font-size: 1.5rem;
}

.nav-items a{
    color: rgb(97, 139, 34);
    text-transform: capitalize;
}
.nav-items > a + a{
    margin-left: 20px;
}
</style>