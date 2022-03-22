<template>
    <nav>
        <a v-for="section in Sections" v-bind:href="'#' + section">
            {{section}}
        </a>
    </nav>
</template>

<script>

export default {
    props: ['Sections'],
    data() {
        return {
            item: "Hello world 2"
        }
    }
}
</script>


<style>
nav {
    position: fixed;
    top: 0%;
    width: 100%;
    padding-top: 15px;
    padding-bottom: 15px;
    display:flex;
    align-items: center;
    justify-content: space-evenly;
    font-family: 'Barlow', sans-serif;
    border-radius: 8px;
    background-color: white;
    
}

nav a {
    text-decoration: none;
    color: black;
    font-size: 1.2em;
    font-weight:bold;
}

nav a:hover{
    color: crimson;
}

</style>