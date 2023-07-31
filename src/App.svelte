<script>
    import Panel from "./Panel.svelte";
    import Card from "./Card.svelte";
    let name ='Wakka'

    let character

    function message(e){
        console.log(e.detail)
    }
</script>

<Panel on:create={message}/>
{#if character}
    <Card {character}/>
{/if}




