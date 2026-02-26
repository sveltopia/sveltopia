<script lang="ts">
	import { MapPin, Palette, Layers } from 'lucide-svelte';
</script>

<svelte:head>
	<title>Sveltopia &mdash; Open-Source Svelte Tools</title>
	<meta name="description" content="Open-source tools for building beautiful Svelte applications" />
	<meta property="og:title" content="Sveltopia — Open-Source Svelte Tools" />
	<meta property="og:description" content="Open-source tools for building beautiful Svelte applications" />
</svelte:head>

<div class="mx-auto max-w-5xl px-6">
	<!-- Hero -->
	<section class="py-24 text-center sm:py-32">
		<h1 class="font-serif text-5xl font-bold tracking-tight text-foreground sm:text-6xl">
			Sveltopia
		</h1>
		<p class="mx-auto mt-6 max-w-2xl text-lg text-muted-foreground sm:text-xl">
			Open-source tools for building beautiful Svelte applications
		</p>
	</section>

	<!-- Product Cards -->
	<section class="grid gap-6 pb-24 sm:grid-cols-2 lg:grid-cols-3">
		<!-- Regions -->
		<a
			href="https://regions.sveltopia.dev"
			class="group rounded-xl border border-slate-200 p-6 transition-all hover:border-indigo-500 hover:shadow-md dark:border-slate-300 dark:hover:border-indigo-700"
		>
			<div class="mb-4 flex items-center gap-3">
				<div class="flex h-10 w-10 items-center justify-center rounded-lg bg-primary-100 text-primary-800 dark:bg-primary-200 dark:text-primary-800">
					<MapPin size={20} />
				</div>
				<span class="rounded-full bg-secondary-100 px-2.5 py-0.5 text-xs font-medium text-secondary-900 dark:bg-secondary-200 dark:text-secondary-900">
					Live
				</span>
			</div>
			<h2 class="text-lg font-semibold text-foreground">Regions</h2>
			<p class="mt-2 text-sm text-muted-foreground">
				Accessible, type-safe region selector components for country, state, and city data.
			</p>
		</a>

		<!-- Colors -->
		<a
			href="https://colors.sveltopia.dev"
			class="group rounded-xl border border-slate-200 p-6 transition-all hover:border-indigo-500 hover:shadow-md dark:border-slate-300 dark:hover:border-indigo-700"
		>
			<div class="mb-4 flex items-center gap-3">
				<div class="flex h-10 w-10 items-center justify-center rounded-lg bg-primary-100 text-primary-800 dark:bg-primary-200 dark:text-primary-800">
					<Palette size={20} />
				</div>
				<span class="rounded-full bg-secondary-100 px-2.5 py-0.5 text-xs font-medium text-secondary-900 dark:bg-secondary-200 dark:text-secondary-900">
					Live
				</span>
			</div>
			<h2 class="text-lg font-semibold text-foreground">Colors</h2>
			<p class="mt-2 text-sm text-muted-foreground">
				Perceptually uniform color system for Tailwind v4, with APCA contrast checking and theme generation.
			</p>
		</a>

		<!-- UI (Coming Soon) -->
		<div
			class="rounded-xl border border-slate-200 p-6 opacity-60 dark:border-slate-300"
		>
			<div class="mb-4 flex items-center gap-3">
				<div class="flex h-10 w-10 items-center justify-center rounded-lg bg-slate-100 text-slate-600 dark:bg-slate-200 dark:text-slate-700">
					<Layers size={20} />
				</div>
				<span class="rounded-full bg-slate-100 px-2.5 py-0.5 text-xs font-medium text-slate-600 dark:bg-slate-200 dark:text-slate-700">
					Coming Soon
				</span>
			</div>
			<h2 class="text-lg font-semibold text-foreground">UI</h2>
			<p class="mt-2 text-sm text-muted-foreground">
				Beautiful, accessible component library built on Svelte 5 and the Sveltopia design system.
			</p>
		</div>
	</section>
</div>
