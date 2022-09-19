<script>
  import NavBar from "./Components/Shared/NavBar.svelte";
  import Auth from "./Routes/Auth.svelte";
  import Home from "./Routes/Home.svelte";
  import NotFound from "./Routes/NotFound.svelte";
  import Router from 'svelte-spa-router'

  let routes={
    '/': Home,
    '/auth': Auth,
    '*': NotFound
  }


  
</script>

<NavBar />
<main>
  <Router {routes} />

</main>