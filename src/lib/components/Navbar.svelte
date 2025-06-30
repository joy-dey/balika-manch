<script>
	import { onDestroy, onMount } from 'svelte';

	const menuOptions = ['Home', 'About', 'The Problem', 'How it works', 'Stories', 'Contact'];

	let isMenuOpen = $state(false);
	let menuRef = $state(null);
	let buttonRef = $state(null);
	let showButton = $state(false);
	let scrollTimeout;

	function toggleMenu() {
		isMenuOpen = !isMenuOpen;
	}

	function closeMenu() {
		isMenuOpen = false;
	}

	function handleClickOutside(event) {
		if (isMenuOpen && !menuRef.contains(event.target) && !buttonRef.contains(event.target)) {
			closeMenu();
		}
	}

	onMount(() => {
		document.addEventListener('click', handleClickOutside);

		return () => {
			document.removeEventListener('click', handleClickOutside);
		};
	});

	function handleScroll() {
		showButton = true;

		clearTimeout(scrollTimeout);
		scrollTimeout = setTimeout(() => {
			if (!isMenuOpen) showButton = false;
		}, 1500); // 2 seconds after scroll stops
	}

	onMount(() => {
		window.addEventListener('scroll', handleScroll);

		return () => {
			window.removeEventListener('scroll', handleScroll);
		};
	});
</script>

<header class="fixed top-2 z-50 w-full">
	<div
		class="container mx-auto flex justify-between rounded-full bg-white py-2.5 pr-2.5 pl-6 shadow"
	>
		<img src="image/logo.svg" alt="" />
		<nav class="hidden space-x-2.5 py-2.5 md:block">
			{#each menuOptions as option}
				<a
					href={`#${option.split(' ').join('-').toLowerCase()}`}
					class="last-of-type:bg-maroon-flush-500 hover:bg-maroon-flush-500 focus:border-maroon-flush-500 rounded-4xl border border-dashed border-transparent px-3 py-2.5 font-medium capitalize last-of-type:text-white hover:text-white focus:outline-0"
					>{option}</a
				>
			{/each}
		</nav>
	</div>
</header>

{#if isMenuOpen}
	<nav
		bind:this={menuRef}
		class="fixed bottom-32 left-1/2 z-50 flex w-full max-w-sm -translate-x-1/2 translate-y-0 flex-col space-x-2.5 rounded-4xl border border-zinc-300 bg-white p-6 shadow-lg transition-transform duration-150 ease-linear starting:translate-y-full"
	>
		{#each menuOptions as option}
			<a
				href={`#${option.split(' ').join('-').toLowerCase()}`}
				onclick={() => closeMenu()}
				class=" hover:bg-maroon-flush-500 focus:border-maroon-flush-500 rounded-4xl border border-dashed border-transparent px-3 py-2.5 text-lg font-medium capitalize hover:text-white focus:outline-0"
				>{option}</a
			>
		{/each}
	</nav>
{/if}

<button
	onclick={() => toggleMenu()}
	bind:this={buttonRef}
	class="from-maroon-flush-500 to-maroon-flush-700 group fixed bottom-4 left-1/2 z-50 flex -translate-x-1/2 flex-col items-center justify-center gap-1.5 rounded-3xl bg-gradient-to-b p-4 text-white transition-all duration-200 ease-in-out md:hidden starting:scale-100 starting:opacity-100"
	aria-label="menu toggler"
	class:opacity-0={!showButton}
	class:scale-0={!showButton}
	class:pointer-events-none={!showButton}
>
	<div class="rounded-lg bg-white/10 p-2">
		<svg
			xmlns="http://www.w3.org/2000/svg"
			viewBox="0 0 24 24"
			fill="currentColor"
			class="h-7 w-7 -rotate-90 fill-white transition-transform duration-200 ease-in-out"
			class:rotate-90={isMenuOpen}
			><path
				d="M17 4H3V6H17V4ZM13 11H3V13H13V11ZM17 18H3V20H17V18ZM15.9896 8.81412L17.4038 7.3999L22 11.9961L17.4038 16.5923L15.9896 15.1781L19.1716 11.9961L15.9896 8.81412Z"
			></path></svg
		>
	</div>
	<span>Menu</span>
</button>
