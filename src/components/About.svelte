<script>

let someText = `Fronted Developer at chrystian.dev`
let count = 0

function handleClick(){
    count++
}

</script>
<style>
p{
    color: var(--theme-color)
}
</style>

<div class="About">
<p>
    {someText}
</p>
<button on:click={handleClick}>Click {count === 0 ? '' : count}</button>
</div>