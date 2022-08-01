<script>
  import { Router, Link, Route } from "svelte-routing";
import About from "./About.svelte";
  import Home from "./Home.svelte";

  export let url = "";
</script>

<Router url="{url}">
  <nav>
  </nav>
  <div>
    <Route path="/"><Home /></Route>
    <Route path="/about"><About /></Route>
  </div>
</Router>
