<script lang="ts">
  import Footer from "lib/components/Footer.svelte";
  import Header from "lib/components/Header.svelte";
  import Metrics from "lib/components/Metrics.svelte";
  import Testimonials from "lib/components/Testimonials.svelte";
  import Vagas from "lib/components/Vagas.svelte";
</script>

<Header />
<Metrics />
<Vagas />
<Testimonials />
<Footer />

<style>
  :global(.btn) {
    font-size: var(--fs-400);
    font-weight: var(--fw-medium);
    background-color: var(--cls-red-500);
    border: none;
    padding: 0.625rem 1.125rem;
    cursor: pointer;
    border-radius: 8px;
    color: #ffffff;
    outline: none;
  }

  :global(.btn):hover,
  :global(.btn):focus {
    background-color: hsl(0, 60%, 50%);
  }

  :global(.chip) {
    --cls-background: var(--cls-red-200);
    mix-blend-mode: multiply;
    padding: 4px 12px;
    color: var(--cls-red-500);
    background-color: var(--cls-background);
    font-weight: var(--fw-semibold);
    font-size: var(--fs-350);
    border-radius: 1rem;
  }

  :global(.chip[data-type="text"]) {
    --cls-background: transparent;
  }
</style>
