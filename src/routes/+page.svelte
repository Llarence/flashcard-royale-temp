<script lang="ts">
	// Combined imports
	import logo from '$lib/images/logo.png';
	import logoFallback from '$lib/images/logo.png';
	import { goto } from '$app/navigation';
</script>

<svelte:head>
	<title>Flashcard Royale - Learn and Compete</title>
	<meta
		name="description"
		content="Drop in. Gear up. Test your knowledge in the ultimate flashcard battle royale experience."
	/>
</svelte:head>

<section
	class="flex min-h-screen flex-col items-center justify-center bg-blue-200 p-16 text-center text-blue-900"
>
	<div class="logo mb-4">
		<picture>
			<source srcset={logo} type="image/webp" />
			<img src={logoFallback} alt="Battle Royale Logo" class="mx-auto h-100" />
		</picture>
	</div>

	<h1 class="mb-4 text-5xl font-bold text-blue-900">Flashcard Royale</h1>

	<h2 class="mb-6 text-2xl text-blue-800">Drop in. Gear up. Fight to be the last one standing.</h2>

	<div class="flex gap-4">
		<a
			href="/play"
			class="rounded-lg bg-blue-700 px-6 py-3 text-base font-bold text-white transition-colors hover:bg-blue-800"
		>
			Play Now
		</a>
		<a
			href="/leaderboard"
			class="rounded-lg bg-blue-700 px-6 py-3 text-base font-bold text-white transition-colors hover:bg-blue-800"
		>
			Leaderboard
		</a>
	</div>
</section>
