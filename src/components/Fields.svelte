<script>
    import Field from "./Field.svelte";
    import Navbar from "./Navbar.svelte";
    import Welcome from "./Welcome.svelte";
    export let fields
</script>

<Navbar />

<Welcome />

{#each fields as field }
    <Field {field}/>
{/each}
