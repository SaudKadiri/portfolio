<script>
    import Card from "./Card.svelte";
    import About from "./About.svelte";
    import Skills from "./Skills.svelte";
    import Projects from "./Projects.svelte";
    import Education from "./Education.svelte";
    import Contact from "./Contact.svelte";
    export let field
</script>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

<div id="{field.id}">
    <Card>
        <h3>{field.title}</h3>
        {#if field.id === 'about'}
            <About />
        {:else if field.id === 'skills'}
            <Skills />
        {:else if field.id === 'projects'}
            <Projects />
        {:else if field.id === 'education'}
            <Education />
        {:else if field.id === 'contact'}
            <Contact />
        {/if}
        <p>{@html field.description}</p>
    </Card>
</div>