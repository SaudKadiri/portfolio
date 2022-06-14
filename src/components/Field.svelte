<script>
    import Card from "./Card.svelte";
    export let field
    let src = "src/routes/saud-dnyandeep.jpg"
</script>

<Card>
    <h3>{field.title}</h3>
    {#if field.title === 'About'}
        <img {src} class="img" alt="Saud's selfie at his favorite place." height="250dp"/>
    {/if}
    <br>
    <p><em>{field.description}</em></p>
</Card>

<style>
    .img {
        border: 1px solid black;
        border-radius: 3px;
        margin-left: 25px;
        margin-right: auto;
    }
</style>