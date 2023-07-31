<script>
    let name = 'World';
    let src = 'https://i.pinimg.com/originals/e2/f3/28/e2f32896f8d03de6ab54f137d8d1c968.gif';
    import Nested from './nested_trial.svelte';
    import EachBlock from './each_block.svelte';
    import Range from './range.svelte';
    import Add from './add_numbers.svelte';
    // import Logo from './logo_svelte.svelte';
    import Slice from './slice_method.svelte';
    import Await from './await.svelte';
    import Event from './event_handler.svelte';
    import Tweening from './tweening.svelte';
    import Fade from './transition.svelte';
    import Transition from './custom_css_transitions.svelte';
    import Stores from './stores.svelte';
</script>

<!-- <Logo/> -->
<section><em><strong>INTRODUCTION</strong></em>
    <h1> Hello {name} !!!</h1>
    <span>Input any value in the box below to change the name-'world'</span><br>
    <input bind:value={name}/>  
    <picture>
    <img id = "image" src={src} alt="thanks gif"> </picture>
</section>
<section><em><strong>REACTIVITY</strong></em>
    <Nested/><br>
    <Add/>
</section>
<section><em><strong>Logic</strong></em>
    <Slice/>
    <EachBlock/>
    <Await/>
</section>

<section><em><strong>Events</strong></em>
    <Event/>

</section>
<section><em><strong>Range</strong></em>
    <Range/> 

    <Transition/>
</section>
<section><em><strong>Tweening</strong></em>
    <Tweening/><br/>
    <Fade/>
</section>
<section><em><strong>Stores</strong></em>
    <Stores/>
</section>

<style>
    picture{
        display:flexbox;
        width:auto;
        height:auto;
        
    }
    span{
        font-size:medium;
        border-style: solid;
        border-color:black;
        border-width: 2px; 
    }
    #image{
        width: 100px;
        height:100px;
        background-color: black;
        margin-top: auto;
    }
    h1{
        color: rgb(47, 78, 255);
        font-family: "sans serif";
        font-size: 50px
        /* margin-below :small; */
    }
    section{
        margin:0 2px;
        padding: 16px 16px;
        width: fit-content;
        /* max-width: 400px; */
        height: fit-content;
        box-sizing: border-box;
        float:left;
        border-style: solid;
        border-width: 2px;
        border-color: black;
    }

</style>