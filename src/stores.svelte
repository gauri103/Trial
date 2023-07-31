<script>import {count} from './stores.js';
import Incrementer from './increment.svelte';
import Decrementer from './decrement.svelte';
import Resetter from './reset.svelte';
let count_value;
count.subscribe((value)=>{
    count_value = value;
});
</script>

<h1>The count is {count_value}</h1>
<Incrementer/>
<Decrementer/>
<Resetter/>
