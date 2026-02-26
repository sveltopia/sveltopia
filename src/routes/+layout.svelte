<script lang="ts">
  import "../app.css";
  import { ModeWatcher } from "mode-watcher";
  import Logo from "$lib/components/Logo.svelte";
  import ThemeSwitcher from "$lib/components/ThemeSwitcher.svelte";

  let { children } = $props();
</script>

<svelte:head>
  <link rel="icon" href="/favicon.svg" />
  <meta property="og:site_name" content="Sveltopia" />
  <meta property="og:type" content="website" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta property="og:image" content="https://sveltopia.dev/og-image.png" />
</svelte:head>

<ModeWatcher />

<div
  class="flex min-h-screen flex-col bg-indigo-100 text-foreground dark:bg-indigo-50"
>
  <!-- Header -->
  <header
    class="sticky top-0 z-40 border-b border-border bg-background/95 backdrop-blur-sm"
  >
    <div class="mx-auto flex h-16 max-w-5xl items-center justify-between px-6">
      <a href="/" class="text-foreground transition-opacity hover:opacity-80">
        <Logo class="h-8" />
      </a>
      <ThemeSwitcher />
    </div>
  </header>

  <!-- Main -->
  <main class="flex-1">
    {@render children()}
  </main>

  <!-- Footer -->
  <footer class="border-t border-border bg-background py-8">
    <div
      class="mx-auto flex max-w-5xl flex-col items-center gap-4 px-6 text-sm text-muted-foreground sm:flex-row sm:justify-between"
    >
      <p>Built by Sveltopia</p>
      <nav class="flex items-center gap-6">
        <a href="/ai-usage" class="transition-colors hover:text-foreground"
          >AI Usage</a
        >
        <a
          href="https://github.com/sveltopia"
          target="_blank"
          rel="noopener noreferrer"
          class="transition-colors hover:text-foreground"
        >
          GitHub
        </a>
      </nav>
    </div>
  </footer>
</div>
