<script>
    import Field from "./Field.svelte";
    import Welcome from "./Welcome.svelte";
    export let fields
</script>

<Welcome />

{#each fields as field }
    <Field {field}/>
{/each}

