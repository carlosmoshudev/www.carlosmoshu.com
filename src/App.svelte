<script lang="ts">
  import { Router, Route } from "svelte-routing";
  import Curriculum from "./Pages/curriculum.svelte";
  import Socialnetworks from "./Pages/socialnetworks.svelte";
  import Skillmatrix from "./Pages/skillmatrix.svelte";
  import Projects from "./Pages/projects.svelte";
  import WebHeader from "./Components/Header/header.svelte";
</script>

<Router>
  <WebHeader />
  <Route path="/" component={Curriculum} />
  <Route path="/socialnetworks" component={Socialnetworks} />
  <Route path="/skillmatrix" component={Skillmatrix} />
  <Route path="/projects" component={Projects} />
</Router>

<style>
</style>
