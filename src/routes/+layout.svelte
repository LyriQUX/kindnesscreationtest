<script>
  import "../app.css";
  import NavBar from "$lib/components/NavBar.svelte";
  import LandingPage from "$lib/components/LandingPage.svelte";
</script>

<main>
  <!-- <LandingPage /> -->
  <NavBar />
  <slot />
</main>