<script>
  import Nav from "./components/Nav.svelte";
  import Hero from "./components/Hero.svelte";
  import PopularProducts from "./components/PopularProducts.svelte";
  import SuperQuality from "./components/SuperQuality.svelte";
  import Services from "./components/Services.svelte";
  import SpecialOffers from "./components/SpecialOffers.svelte";
  import CustomerReviews from "./components/CustomerReviews.svelte";
  import Subscribe from "./components/Subscribe.svelte";
  import Footer from "./components/Footer.svelte";
</script>

<main class="relative">
  <Nav />
  <section class="xl:padding-1 wide:padding-r padding-b">
    <Hero />
  </section>
  <section class="padding bg-blue-400">
    <PopularProducts />
  </section>
  <section class="padding bg-red-400">
    <SuperQuality />
  </section>
  <section class="padding-x py-10 bg-blue-400">
    <Services />
  </section>
  <section class="padding bg-red-400">
    <SpecialOffers />
  </section>
  <section class="bg-pale-blue padding">
    <CustomerReviews />
  </section>
  <section class="padding-x sm:py-32 py-16 w-full bg-red-400">
    <Subscribe />
  </section>
  <section class="padding bg-black padding-x padding-t pb-8">
    <Footer />
  </section>
</main>

<style>
</style>
