<script>
    export let character
</script>

<card>
    <img src={character.src} alt="character">
    <h1>{character.name}</h1>
</card>

<style>
    card{
        background-color: aqua;
        z-index: 9;
    }
</style>