<script>
    import {fade, fly} from 'svelte/transition';
    let visible = true;
</script>
<label>
    <input type="checkbox" bind:checked = {visible}/>
    visible
</label>
<!-- <label>
    <input type="checkbox" bind:checked={visible}/>
    ticked
</label> -->
{#if visible}
<p in:fly={{y:200, duration:2000}} out:fade> 
    flies in and fades out </p>
<!-- <p transition:fly={{y:200, duration:2000}}>
    flies in and out -->
<!-- </p> -->
{/if}
