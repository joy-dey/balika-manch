<script>
	const menuOptions = ['Home', 'About', 'The Problem', 'How it works', 'Stories', 'Contact'];
	const socialLinks = ['Facebook', 'X', 'YouTube', 'Instagram'];
	const logos = [
		'logos/indiagovin.avif',
		'logos/matribandana.avif',
		'logos/poshanabhiyan.avif',
		'logos/towardsanewdawn.avif',
		'logos/childmarriagefree.avif'
	];
</script>

<footer class="text-maroon-flush-50 bg-zinc-950 p-6 pt-16">
	<div class="container mx-auto">
		<div class="flex w-full flex-col items-center justify-center gap-10 text-center">
			<div class="flex flex-col items-center justify-center gap-2.5">
				<img src="image/logo.svg" class="w-40 grayscale invert" alt="" />
				<p class="max-w-sm text-sm opacity-70">
					A school-based movement led by girls, supported by teachers, and backed by the state — to
					end child marriage.
				</p>
			</div>
			<div class="w-full rounded-3xl bg-white/5 p-4">
				<div class="flex flex-wrap items-center justify-center gap-2 md:justify-between">
					<div class="flex flex-wrap gap-2">
						{#each logos as src}
							<img {src} alt="" class="h-10 w-10 last-of-type:w-24" />
						{/each}
					</div>
					<p class="space-x-2 font-sans text-xs font-semibold">
						&copy;2025 Balikamanch. Designed by <a
							href="https://xlayertechnologies.com"
							title="by XLDBF1AA1">xLayer Technologies</a
						>
						<a href="https://storyset.com" class="sr-only font-normal">Illustrations by Storyset</a>
					</p>
				</div>
			</div>
		</div>
	</div>
</footer>
