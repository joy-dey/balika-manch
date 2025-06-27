<script>
	const menuOptions = ['Home', 'About', 'The Problem', 'How it works', 'Stories', 'Contact'];
</script>

<header class="fixed top-1 z-50 w-full">
	<div
		class="container mx-auto flex justify-between rounded-full bg-white py-1.5 pr-2.5 pl-6 shadow"
	>
		<img src="image/logo.svg" alt="" />
		<nav class="space-x-2.5 py-2.5">
			{#each menuOptions as option}
				<a
					href={`#${option.split(' ').join('-').toLowerCase()}`}
					class="hover:bg-maroon-flush-500 focus:border-maroon-flush-500 rounded-4xl border border-dashed border-transparent px-3 py-2.5 capitalize hover:text-white focus:outline-0"
					>{option}</a
				>
			{/each}
		</nav>
	</div>
</header>
