<script>
  import Nav from "./components/Nav.svelte";
  import Hero from "./components/Hero.svelte";
  import PopularProducts from "./components/PopularProducts.svelte";
  import SuperQuality from "./components/SuperQuality.svelte";
  import Services from "./components/Services.svelte";
  import SpecialOffers from "./components/SpecialOffers.svelte";
</script>

<main class="relative">
  <h1 class="text-3xl font-bold underline">Hello world!</h1>
  <Nav />
  <section class="xl:padding-1 wide:padding-r padding-b">
    <Hero />
  </section>
  <section class="padding">
    <PopularProducts />
  </section>
  <section class="padding">
    <SuperQuality />
  </section>
  <section class="padding-x py-10">
    <Services />
  </section>
  <section class="padding">
    <SpecialOffers />
  </section>
  <section class="padding">
    <SpecialOffers />
  </section>
  <section class="padding">
    <SpecialOffers />
  </section>
  <section class="padding">
    <SpecialOffers />
  </section>
</main>

<style>
</style>
