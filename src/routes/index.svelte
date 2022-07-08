<script>
    import global from '../global.css'
    import Fields from "../components/Fields.svelte";
    import Navbar from "../components/Navbar.svelte"
    import { FieldStore } from "../stores";
    let fields = []
    FieldStore.subscribe((data) => fields = data)
</script>

<Navbar {fields}/>
<main class="container">
    <Fields {fields}/>
</main>