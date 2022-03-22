<template>
    <div class="Second_Page" id="Section2">
        <div class="Second_Article">
            <article>
                <h2>
                    {{Content2.Title}}
                </h2>
                <p>
                    {{Content2.Content}}
                </p>
            </article>
        </div>
        <div class="Second_Pic"></div>
    </div>
</template>

<script>
export default {
    props: {
        Content2: Object
    }
}
</script>

<style>
.Second_Page {
    display: grid;
    grid-template-columns: repeat(2, 50%);
    height: 600px;
    background-color: rgb(7, 48, 46);
}

.Second_Article {
    padding: 13px;
    font-size: 1.3em;
    color: white;
    font-family: 'Raleway', sans-serif;
    text-align: right;
    width: 90%;
}

.Second_Pic {
    width: 250px;
    height: 250px;
    border-radius: 100%;
    background-color: white;
}

.Second_Article, .Second_Pic {
    margin: auto;
}


</style>