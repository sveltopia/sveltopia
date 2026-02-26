<script lang="ts">
  import { MapPin, Palette, Layers } from "lucide-svelte";
</script>

<svelte:head>
  <title>Sveltopia &mdash; Open-Source Svelte Tools</title>
  <meta
    name="description"
    content="A growing ecosystem of tools crafted for Svelte developers."
  />
  <meta property="og:title" content="Sveltopia — Open-Source Svelte Tools" />
  <meta
    property="og:description"
    content="A growing ecosystem of tools crafted for Svelte developers."
  />
</svelte:head>

<div class="mx-auto max-w-5xl px-6">
  <!-- Hero -->
  <section class="py-24 text-center sm:py-32">
    <h1
      class="font-serif text-6xl font-bold tracking-tighter text-foreground sm:text-7xl"
    >
      Sveltopia
      <span
        class="mt-1 block h-1 w-12 sm:w-16 mx-auto rounded-full bg-indigo-700 dark:bg-indigo-800"
      ></span>
    </h1>
    <p
      class="mx-auto mt-8 max-w-2xl text-lg text-slate-900 dark:text-slate-900 sm:text-xl"
    >
      A growing ecosystem of tools crafted for Svelte developers.
    </p>
  </section>

  <!-- Product Cards -->
  <section class="grid gap-6 pb-12 sm:grid-cols-2 lg:grid-cols-3">
    <!-- Regions -->
    <a
      href="https://regions.sveltopia.dev"
      class="group rounded-xl border border-slate-300 bg-background p-6 shadow-sm transition-all hover:border-indigo-600 hover:shadow-md dark:border-slate-400 dark:hover:border-indigo-700"
    >
      <div class="mb-4 flex items-center gap-3">
        <div
          class="flex h-10 w-10 items-center justify-center rounded-lg bg-primary-100 text-primary-800 dark:bg-slate-300 dark:text-primary-800"
        >
          <MapPin size={20} />
        </div>
        <span
          class="rounded-full bg-indigo-200 px-2.5 py-0.5 text-xs font-medium text-indigo-900 dark:bg-indigo-200 dark:text-indigo-900"
        >
          Live
        </span>
      </div>
      <h2 class="text-lg font-semibold text-foreground">Regions</h2>
      <p class="mt-2 text-sm text-slate-900 dark:text-slate-900">
        Front Matter for SvelteKit. Named layout regions with runtime schema
        validation.
      </p>
    </a>

    <!-- Colors -->
    <a
      href="https://colors.sveltopia.dev"
      class="group rounded-xl border border-slate-300 bg-background p-6 shadow-sm transition-all hover:border-indigo-600 hover:shadow-md dark:border-slate-400 dark:hover:border-indigo-700"
    >
      <div class="mb-4 flex items-center gap-3">
        <div
          class="flex h-10 w-10 items-center justify-center rounded-lg bg-primary-100 text-primary-800 dark:bg-slate-300 dark:text-primary-800"
        >
          <Palette size={20} />
        </div>
        <span
          class="rounded-full bg-indigo-200 px-2.5 py-0.5 text-xs font-medium text-indigo-900 dark:bg-indigo-200 dark:text-indigo-900"
        >
          Live
        </span>
      </div>
      <h2 class="text-lg font-semibold text-foreground">Colors</h2>
      <p class="mt-2 text-sm text-slate-900 dark:text-slate-900">
        Algorithmic color palettes generated from your brand colors, built on
        OKLCH with APCA contrast validation.
      </p>
    </a>

    <!-- UI (Coming Soon) -->
    <div
      class="rounded-xl border border-slate-200 bg-background p-6 opacity-50 dark:border-slate-300"
    >
      <div class="mb-4 flex items-center gap-3">
        <div
          class="flex h-10 w-10 items-center justify-center rounded-lg bg-slate-100 text-slate-600 dark:bg-slate-200 dark:text-slate-700"
        >
          <Layers size={20} />
        </div>
        <span
          class="rounded-full bg-slate-100 px-2.5 py-0.5 text-xs font-medium text-slate-600 dark:bg-slate-200 dark:text-slate-700"
        >
          Coming Soon
        </span>
      </div>
      <h2 class="text-lg font-semibold text-foreground">UI</h2>
      <p class="mt-2 text-sm text-muted-foreground">
        Beautiful, accessible component library built on Svelte 5 and the
        Sveltopia design system.
      </p>
    </div>
  </section>

  <!-- Philosophy -->
  <section class="pb-24 pt-4">
    <p
      class="mx-auto max-w-2xl text-center text-sm leading-relaxed text-muted-foreground"
    >
      Minimal. Functional. Beautiful.
    </p>
  </section>
</div>
