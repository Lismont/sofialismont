<script>
  import Header from "./Header.svelte";
  import Footer from "./Footer.svelte";
  import Landing from "./Landing.svelte";
  import Werk from "./Werk.svelte";
  import Kontakt from "./Kontakt.svelte";
  import Tabs from "./Tabs.svelte";

  // tabs
  let items = ["Home", "Werk", "Kontakt"];
  let activeItem = "Home";
  const tabChange = e => {
    activeItem = e.detail;
  };
</script>

<main>
<Header />
  <Tabs {activeItem} {items} on:tabChange={tabChange} />

  {#if activeItem === 'Home'}
<Landing />
{:else if activeItem === 'Werk'}
<Werk />
{:else if activeItem === 'Kontakt'}
<Kontakt />
{/if}
  <Footer />
</main>

<style>
</style>