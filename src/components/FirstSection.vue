<template>
    <div class="First_Page" id="Section1">
        <div class="Profile_Pic"></div>
        <div class="Introduction_Bio">
            <article>
                <h2>
                    {{Content.Title}}
                </h2>
                <p>
                    {{Content.Content}}
                </p>
            </article>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        Content: Object
    }
}
</script>

<style >
.First_Page {
    display: grid;
    grid-template-columns: 50% 50%;
    height: 600px;
}

.Profile_Pic {
    border-radius: 100%;
    width: 300px;
    height: 300px;
    margin: auto;
    border: 1px solid gainsboro;
}

.Introduction_Bio {
    margin: auto;
    font-size: 1.3em;
    font-family: 'Raleway', sans-serif;
    width: 90%;
}

</style>