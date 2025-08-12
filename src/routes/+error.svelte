<script>
	import { page } from '$app/state';
	import { slide } from 'svelte/transition';
</script>

<section
	class="bg-maroon-flush-50 flex h-svh flex-col items-center justify-center"
	transition:slide
>
	<h1 class="font-bitter text-maroon-flush-600 text-4xl font-bold md:text-9xl">{page.status}</h1>
	<p class="font-raleway text-center text-lg">
		{#if page.status === 404}
			Looks like you took a wrong turn. But don't worry — we all find our way back.
		{:else}
			We'll fix this. You keep believing in the cause.
		{/if}
	</p>
	<a
		href="/"
		class="border-maroon-flush-200 hover:bg-maroon-flush-600 mt-8 rounded-full border px-6 py-2.5 hover:scale-110 hover:border-transparent hover:text-white"
		>Back to Home</a
	>
</section>
