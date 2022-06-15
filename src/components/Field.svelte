<script>
    import Card from "./Card.svelte";
    import About from "./About.svelte";
    import Skills from "./Skills.svelte";
    export let field
    let src = "src/routes/saud-dnyandeep.jpg"
</script>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

<Card>
    <h3>{field.title}</h3>
    {#if field.title === 'About Me'}
        <About {src}/>
    {:else if field.title === 'Skills'}
        <Skills />
    {/if}
    <br>
    <p>{@html field.description}</p>
</Card>