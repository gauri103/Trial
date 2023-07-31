<script>
    let numbers = [1,2,3,4];
    function add_numbers()
    {
        numbers = [...numbers, numbers.length+1];
    }
    $: sum = numbers.reduce((total, currentnum) => total+currentnum,0 );
</script>
<div id ="add_a_num">
    <br>
    <p>{numbers.join('+')}={sum}</p><br>
    <button on:click={add_numbers}>
    Add a number
    </button>
</div>
