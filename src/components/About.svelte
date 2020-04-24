<script>

let someText = `Fronted Developer at chrystian.dev`
let count = 0

let style = { darkMode: false }

function handleClick(){
    count++
}

function toggle(){
    style.darkMode = !style.darkMode
    window.document.body.classList.toggle("dark-mode")
}

</script>
<style>
p{
    color: var(--theme-color)
}
</style>

<div class="About">

{#if !style.darkMode}
<p>{someText}</p>
{:else}
<p>
<span>Hola Dark Mode</span>
</p>
{/if}


<button on:click={handleClick}>Click {count === 0 ? '' : count}</button>
<button on:click={toggle}>DarkMode</button>
</div>