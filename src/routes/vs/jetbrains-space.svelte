<script>
  import Hero from "$lib/components/jetbrains-space/hero.svelte";
  import FeatureBoxes from "$lib/components/feature-boxes.svelte";
  import { features } from "$lib/contents/jetbrains-space";
  import CalloutSecondary from "$lib/components/callout-secondary.svelte";
  import CompareFeatures from "$lib/components/jetbrains-space/compare-features.svelte";
  import OpenGraph from "$lib/components/open-graph.svelte";
</script>

<OpenGraph
  data={{
    description:
      "Gitpod is the vendor neutral, open-source platform that integrates with your individual stack including all JetBrains IDEs.",
    title: "Gitpod vs JetBrains Space",
    norobots: true,
  }}
/>

<Hero />

<FeatureBoxes {features} />

<CompareFeatures />

<CalloutSecondary
  title="Ready to launch your JetBrains IDE within Gitpod?"
  text="If you already have a Gitpod account, simply go to <a href='https://gitpod.io/preferences'>gitpod.io/preferences</a>, select your favourite IDE and open your project. If you are new to Gitpod, hit the `try now` button."
>
  <img
    src="/images/jetbrains-space/jetbrains-ides-in-gitpod.png"
    alt="Jetbrains IDEs available to use with Gitpod"
    slot="image"
    class="max-w-3xl mx-auto mt-small w-full hidden md:block"
  />
  <img
    src="/images/jetbrains-space/jetbrains-ides-in-gitpod-mobile.png"
    alt="Jetbrains IDEs available to use with Gitpod"
    slot="image-mobile"
    class="max-w-xs mx-auto mt-x-small w-full md:hidden"
  />
</CalloutSecondary>
