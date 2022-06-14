<script>
    import Field from "./Field.svelte";
    import Navbar from "./Navbar.svelte";
    export let fields
</script>

<Navbar />

<h1>Welcome to my website.😊</h1>
<h1>So glad to have you!💛</h1>

{#each fields as field }
    <Field {field}/>
{/each}
