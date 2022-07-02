<script>
    import Card from "./Card.svelte";
    import About from "./About.svelte";
    import Skills from "./Skills.svelte";
    import Projects from "./Projects.svelte";
    import Education from "./Education.svelte";
    import Contact from "./Contact.svelte";
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
    {:else if field.title === 'Projects'}
        <Projects />
    {:else if field.title === 'Education'}
        <Education />
    {:else if field.title === 'Contact Me'}
        <Contact />
    {/if}
    <p>{@html field.description}</p>
</Card>