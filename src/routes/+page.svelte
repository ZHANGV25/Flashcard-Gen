<script>
  import EndlessClouds from '@components/endless-clouds.svelte'
  import Head from '@components/head.svelte'
  import { description, siteName } from '@lib/site-config'
</script>

<Head title={siteName} />

<div class="mb-20 min-h-[65vh] hero">
  <EndlessClouds />
  <div class="bg-opacity-95 hero-overlay" />
  <div class="text-center text-neutral-content hero-content">
    <div class="max-w-2xl">
      <h1 class="font-bold text-secondary mb-5 text-5xl">
        Hello There!
      </h1>
      <h2 class="font-bold text-secondary mb-5 text-4xl">
        Welcome to {siteName}
      </h2>
      <p class="mb-5">
        {description}
      </p>
      <a sveltekit:prefetch href={`/gen`} class="btn btn-primary"
        >Generator</a
      >
    </div>
  </div>
</div>
