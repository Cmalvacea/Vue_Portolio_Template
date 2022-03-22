<template>
    <h1 style="text-align:center;margin-top:15%;font-family:'Barlow',sans-serif;" id="Section3">Contact Media</h1>
    <div class="Contact_Section">
        <div v-for="media in Medias">
            <a :href="media.Link"><ion-icon name="alert-circle-outline"></ion-icon></a>
            <p>
                {{media.MediaName}}
            </p>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        Medias: Array
    }
}
</script>

<style>
.Contact_Section {
    margin: auto;
    margin-top: 10%;
    padding-bottom: 50px;
    display: flex;
    flex-direction: row;
    width: 85%;
    align-items: center;
    justify-content: space-around;
    font-family: 'Barlow', sans-serif;
}

.Contact_Section div {
    display: inherit;
    align-items: center;
    flex-direction: column;
}

.Contact_Section p{
    font-size: 1.5em;
}

.Contact_Section ion-icon {
    font-size: 6em;
}

.Contact_Section a {
    color: black;
}

.Contact_Section a:hover {
    color: gray;
}

</style>