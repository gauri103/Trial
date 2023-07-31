<script>
    import Thing from './thing.svelte';
    let things = [
        { id: 1, name:'apple'},
        { id: 2, name: 'banana'},
        { id: 3, name: 'carrot' },
		{ id: 4, name: 'doughnut' },
		{ id: 5, name: 'egg' }
    ];
    function handleclick() {
        things = things.slice(1);
    }
</script>
    <button on:click={handleclick}>
        Remove first thing
    </button>
    {#each things as thing(thing.id)}
    <Thing name = {thing.name}/>  
    {/each}

   