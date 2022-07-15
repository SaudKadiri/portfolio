<script>
    import Field from "./Field.svelte";
    import Welcome from "./Welcome.svelte";
    import Footer from "./Footer.svelte"
    export let fields
</script>

<Welcome />

{#each fields as field }
    <Field {field}/>
{/each}

<Footer />