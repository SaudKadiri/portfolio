<script>
    import Field from "./Field.svelte";
    export let fields
</script>

{#each fields as field }
    <Field {field}/>
{/each}