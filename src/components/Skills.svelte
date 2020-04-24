<script>
    let skills = [
        {
            id: 1,
            name: 'HTML'
        },
                {
            id: 2,
            name: 'CSS'
        },
                {
            id: 3,
            name: 'JAVASCRIPT'
        },
                {
            id: 4,
            name: 'REAC.JS'
        },
                {
            id: 5,
            name: 'SVELTE'
        },
        
    ]
</script>

<div class="skills">
<h3>Habilidades</h3>
<ul>
{#each skills as skills, i}
<li>{skills.name}</li>
{/each}
</ul>
</div>

<style>
.skills{
    display: flex;
    align-items: center;
    justify-content: center;
}
ul{
    margin: 0;
    padding: 0;
    list-style: none;
}
li {
    display: inline;
    margin: 0 0 0 0.4em;
}

</style>