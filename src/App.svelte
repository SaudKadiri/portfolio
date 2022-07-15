<script>
  import Fields from "./lib/components/Fields.svelte";
  import Navbar from "./lib/components/Navbar.svelte"
  import { FieldStore } from "./lib/stores/stores";
  let fields = []
  FieldStore.subscribe((data) => fields = data)
</script>

<Navbar {fields}/>
<main class="container">
    <Fields {fields}/>
</main>