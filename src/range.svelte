<script>
    let a=1;
    let b=2;
</script>
<label>
    <input type="number" bind:value={a} min= "0" max = "20">
    <input type="range" bind:value = {a} min= "0" max = "20">
</label>
<label>
    <input type="number" bind:value={b} min= "0" max = "20">
    <input type="range" bind:value = {b} min= "0" max = "20">
    <p>{a} + {b} = {a+b}</p>
</label>
<style>
    label{
        margin: 20px;
        border-style: dashed;
        border-color: aqua;
        border-width: 2px;
    }
</style>