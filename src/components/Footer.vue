<template>
    <footer>
        <ul>
            <li>Section 1</li>
            <li>Section 2</li>
            <li>Section 3</li>
            <li>Section 3</li>
        </ul>
        <p>
            Website made by <a href="https://github.com/Cmalvacea" target="_blank">Christopher Malvacea</a>
        </p>
    </footer>
</template>

<style>
footer {
    background-color: rgb(54, 54, 54);
    margin-top: 25%;
    padding: 20px 0px 20px 0px;
    display: flex;
    justify-content: space-evenly;
}

footer ul {
    display: flex;
    flex-direction: column;
    gap: 13px;
}


footer p {
    align-self: center;
}

footer li, footer p, footer a {
    color: gainsboro;
    font-size: 1.2em;
    font-family: 'Barlow', sans-serif;
    text-decoration: none;
    list-style: none;
}
</style>