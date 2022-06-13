<script>
    import global from '../global.css'
    import Fields from "../components/Fields.svelte";

    let fields = ['Programming Languages', 'Frameworks and Tools', 'App development', 'Courses']
</script>

<main>
    <Fields {fields}/>
</main>