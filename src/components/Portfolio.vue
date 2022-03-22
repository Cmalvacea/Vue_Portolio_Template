<template>
<div class="Portfolio_Section" id="Section4">
    <div v-for="skill in Areas" class="Skill_Section">
        <h2>
            {{skill.Skill_Name}}
        </h2>
        <div class="Project_List">
            <div v-for="project in skill.Projects" class="Portolio_Project">
                <div class="Portfolio_Project_Image">
                    <h2>
                        {{project.Project_Name}}
                    </h2>
                </div>
                <div class="Portfolio_Project_Details">
                    <article>
                        <h3>
                            {{project.Project_Name}}
                        </h3>
                        <p>
                            {{project.Project_Details}}
                        </p>
                    </article>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    props: {
        Areas: Array
    }
}
</script>

<style>

.Portfolio_Section {
    margin-top: 15%;
    display: flex;
    flex-direction: column;
    gap: 150px;
    font-family: 'Barlow', sans-serif;
}

.Portfolio_Section h2 {
    padding-left: 10px;
}

.Project_List {
    display: grid;
    grid-template-columns: repeat(4, 25%);
}

.Portfolio_Project_Image {
    text-align: center;
    border: 1px solid gainsboro;
    height: 200px;
}


.Portfolio_Project_Details h3{
    color: rgb(33, 146, 33);
    font-weight: bold;
}

.Portfolio_Project_Details article {
    padding-left: 20px;
}

</style>