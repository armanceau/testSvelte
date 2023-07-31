<script>
    import { createEventDispatcher } from "svelte"
    const dispatch = createEventDispatcher()
    export let name = 'Auron'
    export let src = 'i1.jpg'
    function create(){
        dispatch('create', {name, src})
    }
</script>

<panel>
    <h1>{name}</h1>
    <input bind:value={name}>
    <input bind:value={src}>
    <button on:click={create}>➕</button>

    <br>
    <br>

    <img {src} alt="animal"/>


</panel>

<style>
    panel{
        background-color: aliceblue;
        padding: 10px;
        border-radius: 10px;
    }

    button{
        cursor: pointer;
    }

    img{
        border-radius: 10px;
    }
</style>

