<script>
    // let string = "this string contains a feature of <strong>HTML!!!</strong>"; 
    // export let answer;
    let count = 0;
    $: doubled = count*2;
    function increment(){
        count+=1;
    }
    $:{
    console.log(`the count is ${count}`);
}
    $: if(count >= 5){
    alert("count is dangerously high");
}


</script>
<!-- <p> Trying nested svelte<br></p> -->
<!-- <p>{@html string}</p> -->

<button on:click={increment}>
    Click me 
</button>
<p>I'm clicked {count} {count===1 ? 'time' : 'times'}
    
    doubled of {count} is {doubled}

</p>
<!-- <p> The answer is {answer}</p> -->
{#if count >5}
<p>{count} is relatively high, should not be exceeded</p>
{:else}
<p>{count} is between 0 to 5</p>
{/if}
<style>
    /* p{
        border-style: dashed;
        border-color: aqua;
        border-width: 2px;
    } */
</style>