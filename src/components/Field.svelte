<script>
    import Card from "./Card.svelte";
    import About from "./About.svelte";
    import Skills from "./Skills.svelte";
    export let field
    let src = "src/routes/saud-dnyandeep.jpg"
</script>

<Card>
    <h3>{field.title}</h3>
    {#if field.title === 'About Me'}
        <About {src}/>
    {:else if field.title === 'Skills'}
        <Skills />
    {/if}
    <br>
    <p><em>{field.description}</em></p>
</Card>
