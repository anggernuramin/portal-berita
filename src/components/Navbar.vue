<template>
    <nav>
        <ul>
            <li>
                <a href="">Portal Berita</a>
            </li>
            <li>
                <a href="/"><i class="fa-solid fa-bell"></i></a>
            </li>
        </ul>
    </nav>
</template>

<style scoped>

nav {
    background-color: #295D97;
    width: 100vw;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 9999;
    padding: 20px 0;

}
nav ul{
    list-style-type: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    margin: 0 auto;
    gap: 20px;
}
nav ul li a {
    color: white;
    font-size: 1.3rem;
}
</style>