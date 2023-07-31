<script>
    import {getRandomNumber} from './utils.js';
    let promise = getRandomNumber();
    function handleclick(){
        promise = getRandomNumber();
    } 
</script>
<button on:click={handleclick}>
Get Random Number</button>
{#await promise}
<p>...waiting</p>
{:then number} 
    <p> the number is {number}</p>
{:catch error}
	<p style="color: red">{error.message}</p>
{/await}


