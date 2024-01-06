<script>
  import { arrowRight } from "../assets/icons";
  import { bigShoe1 } from "../assets/images";
  import { statistics, shoes } from "../constants";
  import Button from "./Button.svelte";
  import ShoeCard from "./ShoeCard.svelte";
</script>

<section
  id="home"
  class="w-full flex xl:flex-row flex-col justify-center min-h-screen gap-10 max-container"
>
  <div
    class="relative xl:w-2/5 flex flex-col justify-center items-start w-full max-xl:padding-x pt-28"
  >
    <p class="text-xl font-montserrat text-coral-red">Our Summer Collection</p>
    <h1
      class="mt-10 font-palanquin text-8xl max-sm:text-[72px] max-sm:leading-[82px] font-bold"
    >
      <span class="xl:bg-white xl:whitespace-nowrap relative z-10 pr-10"
        >The New Arrival</span
      >
      <br />
      <span class="text-coral-red inline-block mt-3">Nike</span>
      Shoes
    </h1>
    <p
      class="font-montserrat text-slate-gray text-lg leading-8 mt-6 mb-14 sm:max-w-sm"
    >
      Discover stylish Nike arrivals, quality comfort, and innovation for your
      active life.
    </p>
    <Button iconURL={arrowRight}>Shop Now</Button>

    <div class="flex justify-starts items-start flex-wrap w-full mt-20 gap-16">
      {#each statistics as stat}
        <div>
          <p class="4xl font-palanquin font-bold">{stat.value}</p>
          <p class="leading-7 font-montserrat text-slate-gray">{stat.label}</p>
        </div>
      {/each}
    </div>
  </div>

  <div
    class="relative flex-1 flex justify-center items-center xl:min-h-screen max-xl:py-40 bg-primary bg-hero bg-cover bg-center"
  >
    <img
      src={bigShoe1}
      alt="shoe collection"
      width="610"
      height="500"
      class="object-contain relative z-10"
    />

    <div>
      {#each shoes as shoe}
        <div>
          <!-- <ShoeCard imgURL={shoe} changeBigShoeImage="" bigShoeImg="" /> -->
        </div>
      {/each}
    </div>
  </div>
</section>
