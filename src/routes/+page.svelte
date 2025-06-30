<script>
	const sayings = [
		{
			said: 'If women hold high positions, society will be much more prosperous and developed. Because if mothers and sisters are not protected, no progress can be made.',
			by: {
				name: 'Prof. Dr. Manik Saha',
				image: 'image/manik-saha.avif',
				post: "Hon'ble Chief Minister, Tripura"
			}
		},
		{
			said: "If a girl is forced into marriage before she's ready, we don't just lose a student — we lose a future. Balika Manch was built to stop that from happening.",
			by: {
				name: 'Saju Vaheed',
				image: 'image/saju-vaheed.avif',
				post: 'IAS, District Magistrate'
			}
		}
	];

	const keyStats = [
		{
			value: '21.6%',
			title: 'Girls Married before 19'
		},
		{
			value: '215',
			title: 'Dropouts due to marriage'
		},
		{
			value: '24.1%',
			title: 'Child Marriage Rate in South Tripura'
		},
		{
			value: '2nd',
			title: 'Rank in India for child marriage'
		}
	];

	const teamComposition = [
		{
			image: 'icons/voice-icon.svg',
			title: 'Chairperson',
			description: 'Female teacher who leads and facilitates the club'
		},
		{
			image: 'icons/community-icon.svg',
			title: 'Members',
			description: 'One girl from each class (6-12) who participate actively'
		},
		{
			image: 'icons/star-user.svg',
			title: 'Convenor',
			description: 'Woman from the School Management Committee who advises'
		},
		{
			image: 'icons/parent.svg',
			title: 'Coordinator',
			description: 'Teacher-in-charge, reports issues and ensures action'
		}
	];

	const timelineSteps = [
		{
			image: 'image/social-anxiety.svg',
			title: 'A Concern is Noticed',
			description:
				'It starts with something small — a girl missing school for days, a sudden withdrawal, or signs of fear and pressure at home. These are often red flags noticed by classmates, teachers, or club members. By staying alert to these changes, Balika Manch clubs are able to catch early signs of potential child marriage risks.'
		},
		{
			image: 'image/mobile-inbox.svg',
			title: 'Alert Raised in WhatsApp Group',
			description:
				'Once a concern is identified, the girl-led club’s chairperson or teacher coordinator shares the details in a district-level WhatsApp group. This direct line includes the District Magistrate, child protection officers, and police — ensuring the case is escalated immediately and confidentially, without delays or paperwork.'
		},
		{
			image: 'image/police-car.svg',
			title: 'Authorities Respond in Real-Time',
			description:
				'Within hours, local authorities and protection staff visit the home to speak with the girl and her family. They assess the situation, intervene if a marriage is being planned, and provide counseling to help the family understand the legal and emotional harm. This quick, on-ground response is what prevents the marriage before it can happen.'
		},
		{
			image: 'image/high-school.svg',
			title: 'The Girl is Supported to Rejoin School',
			description:
				'After stopping the marriage, the system doesn’t stop at intervention — it helps her continue her education. Through ₹5,000 financial aid, emotional support from teachers, and encouragement from peers, the girl is reintegrated into school life with dignity and strength. This step ensures she doesn’t just escape harm — she regains her future.'
		}
	];

	const activities = [
		{
			icon: 'icons/chat-smile.svg',
			title: 'Skits & Debates',
			description:
				'Girls create and perform skits, songs, and debates on child rights and gender equality.'
		},
		{
			icon: 'icons/heart-pulse.svg',
			title: 'Health & Hygiene Talks',
			description:
				'Girls create and perform skits, songs, and debates on child rights and gender equality.'
		},
		{
			icon: 'icons/whatsapp.svg',
			title: 'WhatsApp Alerts',
			description:
				'Girls create and perform skits, songs, and debates on child rights and gender equality.'
		},
		{
			icon: 'icons/peer.svg',
			title: 'Peer Support Circles',
			description:
				'Girls create and perform skits, songs, and debates on child rights and gender equality.'
		},
		{
			icon: 'icons/house-smile.svg',
			title: 'Family Counseling',
			description:
				'Girls create and perform skits, songs, and debates on child rights and gender equality.'
		},
		{
			icon: 'icons/rupee.svg',
			title: 'School Rejoining Aid',
			description:
				'Girls create and perform skits, songs, and debates on child rights and gender equality.'
		}
	];

	const videoURLS = [
		'https://www.youtube-nocookie.com/embed/jGCZJbWg5UA?si=VDkE0UKacO4MUzTC&amp;controls=0',
		'https://www.youtube-nocookie.com/embed/_jH1ZdUPaXw?si=UntbIGUCKRV6yzNi&amp;controls=0',
		'https://www.youtube-nocookie.com/embed/nvAlpmvE5xs?si=n94zhJQM-Tq-LJRG&amp;controls=0'
	];

	const impactStats = [
		{
			title: 'Clubs Established',
			value: 346,
			description: 'Balika Manch clubs have been activated in schools across Tripura.',
			icon: 'community-line'
		},
		{
			title: 'Girls Reached',
			value: 12540,
			description: 'Girls who received awareness, peer support, or training through the clubs.',
			icon: 'user-smile-line'
		},
		{
			title: 'Children Counselled',
			value: 2173,
			description: 'At-risk children who were identified and supported through early intervention.',
			icon: 'user-heart-line'
		},
		{
			title: 'Marriages Prevented',
			value: 468,
			description:
				'Child marriages that were stopped thanks to timely alerts and district response.',
			icon: 'shield-check-line'
		}
	];
</script>

<svelte:head>
	<title>Balika Manch | A Girl-Led Movement in Tripura</title>
	<meta
		name="description"
		content="Balika Manch is a girl-led, school-based movement in Tripura that empowers students to prevent child marriages and support each other through education."
	/>

	<!-- Open Graph / Facebook -->
	<meta property="og:type" content="website" />
	<meta property="og:url" content="https://balikamanch.org" />
	<meta property="og:title" content="Balika Manch - A Girl-Led Movement in Tripura" />
	<meta
		property="og:description"
		content="Balika Manch is a girl-led, school-based movement in Tripura that empowers students to prevent child marriages and support each other through education."
	/>
	<meta property="og:image" content="https://balikamanch.org/og.png" />

	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
	<link
		href="https://fonts.googleapis.com/css2?family=Bitter:ital,wght@0,100..900;1,100..900&family=Raleway:ital,wght@0,100..900;1,100..900&display=swap"
		rel="stylesheet"
	/>
</svelte:head>

<!-- landing section -->
<section
	class="bg-maroon-flush-50 flex min-h-[110vh] items-center justify-center bg-[url(image/smiling-school-girls.avif)] bg-cover p-6 py-16 bg-blend-overlay"
	id="home"
>
	<div class="container mx-auto">
		<div class="flex flex-col items-center justify-center gap-10 pt-6 lg:flex-row">
			<div class="col-span-12 content-center space-y-6 landscape:col-span-6">
				<h1 class="font-bitter text-maroon-flush-900 text-5xl font-bold md:text-6xl lg:text-7xl">
					Where Girls Rise — Not as Brides, But as Leaders
				</h1>
				<p>
					Balika Manch is a school-based initiative in Tripura that empowers girls to stay in
					school, speak up, and prevent child marriages — through community, support, and courage.
				</p>
				<blockquote class="w-fit rounded-2xl bg-white p-6">
					<p class="font-bitter text-xl leading-tight font-medium italic">
						“I didn't know I had a choice — until Balika Manch showed me.”
					</p>
					<cite class="text-maroon-flush-500 text-sm not-italic"
						>- Rupa, Class 8, South Tripura</cite
					>
				</blockquote>
				<div class="flex gap-4">
					<button class="bg-maroon-flush-600 rounded-full p-2.5 px-5 font-semibold text-white"
						>Join the movement</button
					>
					<button class="text-maroon-flush-600 font-semibold">See the impact</button>
				</div>
			</div>
			<div class="col-span-12 flex w-full flex-col landscape:col-span-6">
				<img src="image/photo-collage.avif" alt="" class="h-auto w-11/12" />
				<div class="mt-8 flex flex-wrap gap-4 lg:flex-nowrap">
					<div class="flex w-full items-center gap-2 rounded-full bg-white px-6 py-4">
						<p class="text-maroon-flush-600 text-3xl font-bold">450+</p>
						<p class="text-sm capitalize">child marriages prevented</p>
					</div>
					<div class="flex w-full items-center gap-2 rounded-full bg-white px-6 py-4">
						<p class="text-maroon-flush-600 text-3xl font-bold">500+</p>
						<p class="text-sm capitalize">girls supported to stay in school</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>

<!-- about section -->
<section class="scroll-m-10 p-6 py-16" id="about">
	<div class="container mx-auto">
		<!-- info -->
		<div class="flex flex-col gap-8 md:flex-row">
			<div class="items-stretch md:w-1/2 lg:w-4/12">
				<img
					src="image/ias-saju-giving-speech.avif"
					alt="IAS Saju giving speech"
					class="h-full w-full rounded-3xl object-cover object-left"
				/>
			</div>
			<div class="group md:w-1/2 lg:w-8/12">
				<h2 class="font-bitter mb-4 text-4xl font-medium">
					<span class="text-maroon-flush-600 block">Balika Manch</span> Led by Girls, Backed by Leaders
				</h2>
				<div class="space-y-2 text-zinc-600">
					<p>
						Balika Manch is a girl-led, school-based initiative under the Beti Bachao, Beti Padhao
						scheme, working to prevent child marriage and ensure that every girl in Tripura has the
						right to stay in school and shape her own future.
					</p>
					<p>
						Originally launched in 2020, the program was revived in 2022 by IAS officer Saju Vaheed,
						then District Magistrate of South Tripura. His leadership brought new life to the
						initiative, empowering schools, teachers, and students to intervene early — preventing
						over 150 child marriages in just one year.
					</p>
					<p>
						The movement is supported by the Government of Tripura and the Hon’ble Chief Minister,
						Dr. Manik Saha, whose commitment to girl child education and empowerment has made Balika
						Manch a model of community-led impact.
					</p>
				</div>
			</div>
		</div>
		<!-- quotes -->
		<div class="grid grid-cols-1 gap-10 py-10 md:grid-cols-2">
			{#each sayings as saying}
				<div>
					<blockquote class="font-bitter text-2xl font-medium">
						<span class="text-maroon-flush-600 font-bitter text-6xl font-medium text-balance"
							>“</span
						>{saying.said}”
						<div class="font-raleway mt-6 flex items-center gap-4">
							<img
								src={saying.by.image}
								alt={`Photo of ${saying.by.name}`}
								class="h-20 w-20 rounded-xs"
							/>
							<div class="flex flex-col">
								<cite class="text-xl font-semibold not-italic">{saying.by.name}</cite>
								<small class="text-sm text-zinc-500">{saying.by.post}</small>
							</div>
						</div>
					</blockquote>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- challenge we are facing section -->
<section class="scroll-m-10 p-6 py-16" id="the-problem">
	<div class="container mx-auto">
		<h3
			class="font-bitter after:bg-maroon-flush-600 mb-4 text-4xl font-medium after:ml-3 after:inline-block after:h-1 after:w-20 after:-translate-y-1/2 after:content-['']"
		>
			<span class="text-maroon-flush-600"> The Challenge </span> We're Facing
		</h3>
		<p>
			Tripura has the second-highest rate of child marriage in India. More than 1 in 5 girls between
			the ages of 15 and 19 are married — often dropping out of school and losing their chance to
			choose their future. In some districts, nearly a quarter of girls never make it past secondary
			school because of early marriage.
		</p>
		<div class="mt-6 grid grid-cols-2 py-2.5 md:grid-cols-2 lg:grid-cols-4">
			{#each keyStats as { title, value }}
				<div class="space-y-2.5 p-2.5">
					<p class="text-maroon-flush-600 font-bitter text-4xl font-medium">{value}</p>
					<span class="text-sm">{title}</span>
				</div>
			{/each}
		</div>
		<!-- highlight -->
		<div class="grid grid-cols-1 gap-6 py-5 md:grid-cols-2">
			<blockquote class="bg-maroon-flush-50 h-full content-center rounded-3xl p-10">
				<p class="text text-maroon-flush-500 font-bitter text-2xl font-semibold">
					Every statistic hides a story — of a girl forced to leave school, of a childhood
					interrupted too soon. We believe every girl deserves to grow, to learn, and to lead her
					own life.
				</p>
			</blockquote>
			<div class="">
				<img
					src="image/image-of-a-small-girl-showing-hena.avif"
					alt=""
					class="rounded-3xl grayscale"
				/>
			</div>
		</div>
	</div>
</section>

<!-- how it works -->
<section class="bg-maroon-flush-50 scroll-m-10 p-6 py-16" id="how-it-works">
	<div class="container mx-auto">
		<h3
			class="font-bitter after:bg-maroon-flush-600 mb-4 text-4xl font-medium after:ml-3 after:inline-block after:h-1 after:w-20 after:-translate-y-1/2 after:content-['']"
		>
			<span class="text-maroon-flush-600">A Girl-Led Movement,</span> Built in Every School
		</h3>
		<p>
			Balika Manch is a school-based girls’ club designed to empower students, raise awareness, and
			prevent child marriage — right from within the classroom. Each club is led by a female teacher
			and includes one girl from each class (6–12), supported by the school’s management committee.
			Together, they create a safe, informed, and responsive space for girls to speak up, support
			one another, and act early when risks arise.
		</p>

		<div class="pt-10">
			<h4 class="font-bitter text-2xl font-semibold">
				<span class="text-maroon-flush-600">Meet the Team</span> Behind Every Club
			</h4>
			<p>
				Each Balika Manch club is powered by girls, guided by teachers, and supported by school
				leadership.
			</p>

			<div class="grid grid-cols-1 py-10">
				<div class="grid grid-cols-1 gap-2 md:grid-cols-4">
					{#each teamComposition as { image, title, description }}
						<div class=" space-y-2.5 rounded-2xl bg-white p-4">
							<div
								class="bg-maroon-flush-400 flex h-11 w-11 items-center justify-center rounded-lg"
							>
								<img src={image} alt="" class="h-6 w-6" />
							</div>
							<p class="text-xl font-semibold">{title}</p>
							<span class="block leading-tight text-balance text-zinc-500">{description}</span>
						</div>
					{/each}
				</div>
			</div>
		</div>
		<div class="pt-10">
			<div class="flex w-full flex-col gap-10">
				<div class="group">
					<h4 class="font-bitter text-3xl font-semibold">
						<span class="text-maroon-flush-600">From Concern</span> to Action
					</h4>
					<p class="mb-4 text-xl">How Balika Manch Clubs Intervene to Protect Girls</p>
				</div>
				<div class="grid grid-cols-1 gap-10 md:grid-cols-2">
					{#each timelineSteps as { image, title, description }}
						<div class="flex flex-col flex-wrap gap-4">
							<div class="w-6/12 rounded-4xl bg-white/5">
								<img src={image} alt="" class="w-full" />
							</div>
							<div class="w-full space-y-2.5">
								<p class="text-3xl font-semibold">{title}</p>
								<span class="block text-lg text-zinc-500">{description}</span>
							</div>
						</div>
					{/each}
				</div>
			</div>
		</div>
		<div
			class="border-maroon-flush-500 mt-16 mb-16 flex flex-col items-center gap-4 rounded-3xl border-l-4 bg-white p-4 md:flex-row"
		>
			<img src="image/brain.svg" alt="" />
			<div class="space-y-2">
				<p class="font-bitter text-3xl font-semibold">Did you know?</p>
				<p>
					Balika Manch clubs can directly trigger emergency intervention through district WhatsApp
					groups — connecting teachers, child protection, and police within minutes.
				</p>
			</div>
		</div>

		<div class="pt-10">
			<h3
				class="font-bitter after:bg-maroon-flush-600 mb-4 text-4xl font-medium after:ml-3 after:inline-block after:h-1 after:w-20 after:-translate-y-1/2 after:content-['']"
			>
				Where <span class="text-maroon-flush-600">the Movement Lives</span>
			</h3>
			<p>
				Balika Manch isn't an idea — it's active in schools across Tripura, supporting hundreds of
				girls every day.
			</p>
			<div class="mt-10 grid grid-cols-1 gap-y-10 lg:grid-cols-2">
				<svg
					viewBox="0 0 800 1074"
					fill="none"
					xmlns="http://www.w3.org/2000/svg"
					class="mx-auto w-80"
				>
					<mask id="path-1-inside-1_78_1665" fill="white">
						<path
							fill-rule="evenodd"
							clip-rule="evenodd"
							d="M495.87 731.62L483.37 726.91L481.9 723.82L484.99 717.1L470.07 716.16L464.43 708.37H457.58L450.86 716.84L458.25 725.84L462.68 735.51L458.79 743.84L450.32 742.23L443.47 749.62L442.39 737.66L433.26 744.51L429.9 737.66V730.94L424.92 711.73L410.14 701.52L408.94 694.8L402.75 687.95L401.68 671.55L384.75 678.94L377.9 669.27L384.21 663.63L390.39 664.7L397.11 660.8L393.21 646.16L380.72 643.87L380.18 635.41L376.82 619.55L380.72 594.7L379.64 581.66L376.28 577.63V571.45L368.36 570.91L364.33 566.35L372.25 548.21V535.84L370.24 523.35H373.06L376.96 518.38L379.78 519.18L380.85 524.29L382.73 525.09L384.62 530.94L392.27 535.17L396.17 538.53L397.11 544.31L398.99 545.25L399.06 549.42L397.11 554.39L391.47 559.36L389.59 563.52L390.53 565.14L396.24 568.56L398.12 572.79L401.95 576.15L402.96 581.13L411.62 572.79L421.16 571.18L423.98 567.02L422.98 560.03L420.09 556.67L421.9 554.18L420.09 548.21L429.56 532.48L424.72 527.45L420.76 513.2V506.55L423.58 499.83L421.7 493.92L426.4 490.7V489.02H422.57L415.79 478.13L421.57 480.62L423.45 479.81L426.34 480.69L427.21 470.54L426.27 463.96L427.07 446.36L428.89 438.03L424.12 433.86L425.06 428.82L423.04 418.81L412.56 413.71L411.62 407.93L415.52 404.57L413.77 402.02L412.43 391.13L407.86 388.58L410.01 377.83L408.06 368.63L411.15 352.3L411.76 341.28L409.14 334.03L410.14 329.05L408.4 317.9L409.67 315.48L409 313.27L405.78 310.24L409.61 299.76L408.53 283.03L412.16 266.24L408.87 263.89L411.09 264.36L411.22 262.01L401.61 193.88L432.32 211.28L439.84 212.29L442.46 211.42L443 212.56L442.19 212.76L445.28 213.5L446.69 217.06L448.57 217.26L449.25 218.61L454.15 218.54L456.03 216.12L457.91 216.46L459.26 213.1L463.42 212.16L463.15 208.13L467.79 205.84L470.21 206.38L468.33 208.06L469.13 209.2L466.98 210.14L467.18 211.69L472.89 210.95L476.52 215.78L473.43 215.58L475.31 216.52L475.04 217.46L471.75 216.72L473.23 219.75L471.35 219.68L471.08 220.69L472.15 220.62L471.82 223.85L470.21 225.39L467.79 223.98L466.44 224.38L467.92 225.46L467.79 227.47L468.66 227.07L468.33 228.28L469.94 229.96L468.39 232.18L469.74 232.65L470.54 235.47L471.42 235.2L473.43 237.69L474.71 236.41L475.72 236.61L475.58 237.75H478.87L479.34 236.88L479.28 237.69L482.03 238.69L482.64 241.05L484.85 240.64L486.33 242.46H487.94L487.61 244.81L488.95 244.61L489.56 245.61L487.54 246.89L488.48 247.16L487.74 247.56L488.61 248.7L487.81 250.05L489.76 251.19L490.16 253.81L489.29 254.68L491.37 257.91L491.03 261.27L492.85 261.74L494.93 265.03L498.62 267.45L502.59 265.63L506.96 267.65L514.55 279.61L515.08 282.43L513.74 284.98L526.77 294.66L539.54 299.23L552.84 311.05L558.62 310.51L573.8 300.7L577.43 297.08L585.36 296.27L612.77 290.09L613.17 320.32L618.68 330.4L615.99 339L605.11 342.89L604.44 350.55L608.07 356.33V361.97L610.35 365.87L616.53 364.26L622.71 365.06L626.88 369.23L634.4 370.98L634.27 377.02L638.16 380.52L639.78 384.01L638.43 389.79L634.67 396.91L635.61 401.61L641.79 402.02L645.82 404.43L652.54 405.78L659.26 403.9L662.35 406.45L665.57 415.32L667.05 426.34L671.62 432.92L679.28 459.93L679.01 467.99L677.94 469.47L678.47 481.29L679.55 484.79L680.35 506.42L682.24 513.41L680.35 516.9L680.09 520.12L681.43 523.35L686.8 523.89L689.36 525.23L690.97 528.32L689.49 532.48L679.01 535.64L676.66 538.2L672.49 537.32L669.54 539L668.13 544.24L665.64 547.2L666.18 547.67L662.55 550.69L659.33 555.93L656.77 556.87L656.44 560.7L655.23 561.58L655.83 564.13L643.81 577.09L641.86 577.5L635.28 575.75L634.33 576.69L631.45 574.27L630.84 575.01L629.83 574.14L628.49 574.68L626.81 580.52L625.33 580.72L623.92 582.8L626.41 586.63L625.94 590.93L624.93 591.87L625.94 595.77L621.3 596.98L619.08 596.04L615.25 598.19L611.36 595.84L606.12 595.3L603.56 597.05L599.74 595.7L599.06 594.02L595.57 592.48L592.55 589.19L587.51 589.39L588.92 587.31L588.25 586.16L582.47 587.98L581.33 585.76L578.3 585.69L576.89 580.86L574.88 580.18L573 580.99L572.06 575.95L570.44 574.81L569.3 569.7L568.5 569.57L568.56 566.08L565.14 560.5L565.2 558.01L562.65 550.22V545.85L561.91 545.12L559.83 545.79L557.95 538.93L557.34 539.88L547.2 542.7L543.57 548.47L544.65 552.51L543.44 556.74L543.97 565.34L541.55 565.74L535.17 571.18L533.9 573.53L539.14 589.46L540.35 596.98L539.74 606.39L543.57 616.46L541.62 633.06L542.7 635.21L541.82 637.29L545.12 637.69L548.41 642.73L546.12 650.59L549.62 659.33L547.13 667.99L548.81 671.89L548.14 673.3L545.05 673.91L543.23 678.34L545.85 683.18L548.74 682.97L547.94 683.92L548.61 684.99L551.23 686.4L551.83 689.63L555.39 692.78L553.65 696.08L554.32 697.76L556.6 698.36L554.32 701.99L556 707.5L554.72 708.5L552.1 708.03L551.9 711.46L550.69 710.39L544.58 709.31L544.91 713.74L543.37 711.86L542.5 712.13L540.35 715.49L537.46 716.03L537.59 717.98L536.11 718.51L535.44 717.31L533.96 718.04L533.36 721.94L537.25 733.23L534.16 737.12V739.21L532.69 739.01L530.6 741.02L528.45 740.21L528.86 739.14L527.71 738.67L521.6 740.15L520.12 737.26L517.84 736.18L514.48 738.07L509.84 738L505.21 735.51V737.06L495.87 731.62ZM490.63 258.58L490.56 258.71L490.63 258.78V258.71V258.58Z"
						/>
					</mask>
					<path
						fill-rule="evenodd"
						clip-rule="evenodd"
						d="M495.87 731.62L483.37 726.91L481.9 723.82L484.99 717.1L470.07 716.16L464.43 708.37H457.58L450.86 716.84L458.25 725.84L462.68 735.51L458.79 743.84L450.32 742.23L443.47 749.62L442.39 737.66L433.26 744.51L429.9 737.66V730.94L424.92 711.73L410.14 701.52L408.94 694.8L402.75 687.95L401.68 671.55L384.75 678.94L377.9 669.27L384.21 663.63L390.39 664.7L397.11 660.8L393.21 646.16L380.72 643.87L380.18 635.41L376.82 619.55L380.72 594.7L379.64 581.66L376.28 577.63V571.45L368.36 570.91L364.33 566.35L372.25 548.21V535.84L370.24 523.35H373.06L376.96 518.38L379.78 519.18L380.85 524.29L382.73 525.09L384.62 530.94L392.27 535.17L396.17 538.53L397.11 544.31L398.99 545.25L399.06 549.42L397.11 554.39L391.47 559.36L389.59 563.52L390.53 565.14L396.24 568.56L398.12 572.79L401.95 576.15L402.96 581.13L411.62 572.79L421.16 571.18L423.98 567.02L422.98 560.03L420.09 556.67L421.9 554.18L420.09 548.21L429.56 532.48L424.72 527.45L420.76 513.2V506.55L423.58 499.83L421.7 493.92L426.4 490.7V489.02H422.57L415.79 478.13L421.57 480.62L423.45 479.81L426.34 480.69L427.21 470.54L426.27 463.96L427.07 446.36L428.89 438.03L424.12 433.86L425.06 428.82L423.04 418.81L412.56 413.71L411.62 407.93L415.52 404.57L413.77 402.02L412.43 391.13L407.86 388.58L410.01 377.83L408.06 368.63L411.15 352.3L411.76 341.28L409.14 334.03L410.14 329.05L408.4 317.9L409.67 315.48L409 313.27L405.78 310.24L409.61 299.76L408.53 283.03L412.16 266.24L408.87 263.89L411.09 264.36L411.22 262.01L401.61 193.88L432.32 211.28L439.84 212.29L442.46 211.42L443 212.56L442.19 212.76L445.28 213.5L446.69 217.06L448.57 217.26L449.25 218.61L454.15 218.54L456.03 216.12L457.91 216.46L459.26 213.1L463.42 212.16L463.15 208.13L467.79 205.84L470.21 206.38L468.33 208.06L469.13 209.2L466.98 210.14L467.18 211.69L472.89 210.95L476.52 215.78L473.43 215.58L475.31 216.52L475.04 217.46L471.75 216.72L473.23 219.75L471.35 219.68L471.08 220.69L472.15 220.62L471.82 223.85L470.21 225.39L467.79 223.98L466.44 224.38L467.92 225.46L467.79 227.47L468.66 227.07L468.33 228.28L469.94 229.96L468.39 232.18L469.74 232.65L470.54 235.47L471.42 235.2L473.43 237.69L474.71 236.41L475.72 236.61L475.58 237.75H478.87L479.34 236.88L479.28 237.69L482.03 238.69L482.64 241.05L484.85 240.64L486.33 242.46H487.94L487.61 244.81L488.95 244.61L489.56 245.61L487.54 246.89L488.48 247.16L487.74 247.56L488.61 248.7L487.81 250.05L489.76 251.19L490.16 253.81L489.29 254.68L491.37 257.91L491.03 261.27L492.85 261.74L494.93 265.03L498.62 267.45L502.59 265.63L506.96 267.65L514.55 279.61L515.08 282.43L513.74 284.98L526.77 294.66L539.54 299.23L552.84 311.05L558.62 310.51L573.8 300.7L577.43 297.08L585.36 296.27L612.77 290.09L613.17 320.32L618.68 330.4L615.99 339L605.11 342.89L604.44 350.55L608.07 356.33V361.97L610.35 365.87L616.53 364.26L622.71 365.06L626.88 369.23L634.4 370.98L634.27 377.02L638.16 380.52L639.78 384.01L638.43 389.79L634.67 396.91L635.61 401.61L641.79 402.02L645.82 404.43L652.54 405.78L659.26 403.9L662.35 406.45L665.57 415.32L667.05 426.34L671.62 432.92L679.28 459.93L679.01 467.99L677.94 469.47L678.47 481.29L679.55 484.79L680.35 506.42L682.24 513.41L680.35 516.9L680.09 520.12L681.43 523.35L686.8 523.89L689.36 525.23L690.97 528.32L689.49 532.48L679.01 535.64L676.66 538.2L672.49 537.32L669.54 539L668.13 544.24L665.64 547.2L666.18 547.67L662.55 550.69L659.33 555.93L656.77 556.87L656.44 560.7L655.23 561.58L655.83 564.13L643.81 577.09L641.86 577.5L635.28 575.75L634.33 576.69L631.45 574.27L630.84 575.01L629.83 574.14L628.49 574.68L626.81 580.52L625.33 580.72L623.92 582.8L626.41 586.63L625.94 590.93L624.93 591.87L625.94 595.77L621.3 596.98L619.08 596.04L615.25 598.19L611.36 595.84L606.12 595.3L603.56 597.05L599.74 595.7L599.06 594.02L595.57 592.48L592.55 589.19L587.51 589.39L588.92 587.31L588.25 586.16L582.47 587.98L581.33 585.76L578.3 585.69L576.89 580.86L574.88 580.18L573 580.99L572.06 575.95L570.44 574.81L569.3 569.7L568.5 569.57L568.56 566.08L565.14 560.5L565.2 558.01L562.65 550.22V545.85L561.91 545.12L559.83 545.79L557.95 538.93L557.34 539.88L547.2 542.7L543.57 548.47L544.65 552.51L543.44 556.74L543.97 565.34L541.55 565.74L535.17 571.18L533.9 573.53L539.14 589.46L540.35 596.98L539.74 606.39L543.57 616.46L541.62 633.06L542.7 635.21L541.82 637.29L545.12 637.69L548.41 642.73L546.12 650.59L549.62 659.33L547.13 667.99L548.81 671.89L548.14 673.3L545.05 673.91L543.23 678.34L545.85 683.18L548.74 682.97L547.94 683.92L548.61 684.99L551.23 686.4L551.83 689.63L555.39 692.78L553.65 696.08L554.32 697.76L556.6 698.36L554.32 701.99L556 707.5L554.72 708.5L552.1 708.03L551.9 711.46L550.69 710.39L544.58 709.31L544.91 713.74L543.37 711.86L542.5 712.13L540.35 715.49L537.46 716.03L537.59 717.98L536.11 718.51L535.44 717.31L533.96 718.04L533.36 721.94L537.25 733.23L534.16 737.12V739.21L532.69 739.01L530.6 741.02L528.45 740.21L528.86 739.14L527.71 738.67L521.6 740.15L520.12 737.26L517.84 736.18L514.48 738.07L509.84 738L505.21 735.51V737.06L495.87 731.62ZM490.63 258.58L490.56 258.71L490.63 258.78V258.71V258.58Z"
						stroke="black"
						stroke-width="2"
						class="fill-maroon-flush-300 hover:fill-maroon-flush-500"
						mask="url(#path-1-inside-1_78_1665)"
					/>
					<mask id="path-2-inside-2_78_1665" fill="white">
						<path
							d="M450.19 968.23L437.96 957.75L428.28 945.53L422.1 947.68L409.47 931.42L430.84 934.11L435.67 926.18L433.93 919.19L424.79 909.11L423.04 899.57L410.28 885.6L411.22 876.33L406.79 860.61L399.4 847.44L389.18 836.76L388.24 830.91L392.95 821.64L392.01 817.54L388.24 816.67L386.36 817.48L372.93 803.23L369.03 796.51L370.91 793.22L369.97 789.06H368.02L366.14 791.54L365.27 789.93L367.08 785.7L365.13 784.02L346.99 788.99L339.47 794.77L337.45 788.12L333.69 784.69L330.73 771.39L324.96 772.19V763.86L323.01 758.89L325.9 756.34L323.95 750.49L320.12 745.46L314.34 749.62L310.58 756.34L303.86 757.95L299.16 762.92L293.31 758.76L290.49 757.95L290.42 753.72L288.54 749.55L282.77 746.19L279 745.32L276.99 742.84L268.46 748.75L256.97 751.97L253.14 752.04L249.31 750.29L247.43 751.1V753.65L243.67 756.07L228.28 756.94L224.45 758.62L215.85 757.82L217.73 762.79L216.93 767.76L213.03 767.83L209.27 776.9L197.85 784.42L193.95 783.62L182.6 777.84L182.39 772.73L170.03 767.63L165.2 766.82L160.36 764.4L158.48 761.85V755.13L160.36 748.41V744.25L159.28 741.83L155.52 740.08L153.64 736.72V734.3L155.52 730.94L155.39 725.84L157.27 718.45L161.16 715.89L163.05 711.73L157.27 708.37L158.21 705.01L158.07 697.49L156.19 695.87L154.31 689.96L152.3 688.35L157.13 683.24L167.61 682.44L173.93 685.39L182.53 680.56L196.77 676.39L207.25 678.68L209.67 667.66L196.37 660.54L185.35 666.31L176.75 673.43L168.55 670.75L167.61 662.42L165.6 659.86L168.42 657.45L167.48 650.73L168.42 645.76L167.48 641.59L173.12 639.04L189.38 626.54L194.08 619.82V617.4L192.2 616.46L199.86 610.69L201.74 606.52L207.52 603.16L211.28 591.47L218 587.31L220.82 583.95L224.59 583.14L226.33 587.58L228.21 599.13L235.87 601.01L251.19 589.46L260.19 591.87L270.27 585.69L262.07 567.55L265.97 561.91L277.39 553.71L280.08 540.68L284.92 534.77L286.8 529.8L284.78 527.24L283.84 523.15L286.73 524.02L289.55 523.15L294.39 525.7L301.11 524.02L302.11 521.53L331.81 519.05L333.69 520.8L350.02 521.67L363.52 524.96L366.34 522.54L370.24 523.35L372.25 535.84V548.21L364.33 566.35L368.36 570.91L376.28 571.45V577.63L379.64 581.66L380.72 594.7L376.82 619.55L380.18 635.41L380.72 643.87L393.21 646.16L397.11 660.8L390.39 664.7L384.21 663.63L377.9 669.27L384.75 678.94L401.68 671.55L402.75 687.95L408.94 694.8L410.14 701.52L424.92 711.73L429.9 730.94V737.66L433.26 744.51L442.39 737.66L443.47 749.62L450.32 742.23L458.79 743.84L462.68 735.51L458.25 725.84L450.86 716.84L457.58 708.37H464.43L470.07 716.16L484.99 717.1L481.9 723.82L483.37 726.91L495.87 731.62L506.22 737.93L502.59 740.35L502.25 741.69L499.7 740.21L497.01 740.62L497.82 743.04L496.68 744.72L489.62 747.81L488.01 749.89L487.74 753.32L483.24 755L478.94 759.29L475.04 758.29L472.49 760.03L468.53 759.63L468.73 762.39L465.84 762.92L466.44 770.58L462.61 771.86L463.56 782.41L460.06 783.08L458.79 786.91L457.44 785.5L456.5 786.3L455.49 787.51L455.16 794.77L451.19 795.64L450.39 798.8L443.87 804.04L432.72 822.85L432.99 821.71L421.36 844.75V848.25L420.09 850.13L422.84 850.6L422.64 854.56L421.7 855.5L423.18 856.84L422.78 858.59L421.43 858.93L422.78 860.14L423.58 859.2L424.66 861.01L423.78 862.35L425.06 865.58L422.37 867.53L424.79 870.42L425.66 869.27L425.19 868.06H427.21L428.42 870.89L427.61 872.63L432.99 877.6L431.71 882.71L432.79 884.93L430.17 886.74L432.65 888.82L432.05 889.43L433.39 891.11L434.2 896.21L436.14 898.23L437.89 899.44L438.36 902.13L437.42 905.89L438.97 908.64L442.46 911.13L440.38 912.81L441.05 914.29L442.73 913.75L441.65 914.49L442.93 915.63L442.06 915.97L442.33 917.24L443.27 919.8L445.01 920.6L442.93 922.35L442.33 925.84L445.35 928.33L445.15 929.54L446.49 928.19L447.77 932.63L447.7 934.31L445.68 934.37L443.74 938.07L443.87 940.89L445.35 941.63L445.75 939.55L446.02 941.29L448.17 941.97V943.17L446.56 943.71L450.32 945.79L449.25 948.48L447.36 949.96L447.57 951.57L452.34 949.29L450.39 956.14L453.54 956.54L455.16 959.9L453.34 962.46L453.95 963.8L459.59 964.34L462.14 967.43V969.31H460.46L460.73 970.38L459.32 971.19L458.25 969.91L457.78 970.79L450.19 968.23Z"
						/>
					</mask>
					<path
						d="M450.19 968.23L437.96 957.75L428.28 945.53L422.1 947.68L409.47 931.42L430.84 934.11L435.67 926.18L433.93 919.19L424.79 909.11L423.04 899.57L410.28 885.6L411.22 876.33L406.79 860.61L399.4 847.44L389.18 836.76L388.24 830.91L392.95 821.64L392.01 817.54L388.24 816.67L386.36 817.48L372.93 803.23L369.03 796.51L370.91 793.22L369.97 789.06H368.02L366.14 791.54L365.27 789.93L367.08 785.7L365.13 784.02L346.99 788.99L339.47 794.77L337.45 788.12L333.69 784.69L330.73 771.39L324.96 772.19V763.86L323.01 758.89L325.9 756.34L323.95 750.49L320.12 745.46L314.34 749.62L310.58 756.34L303.86 757.95L299.16 762.92L293.31 758.76L290.49 757.95L290.42 753.72L288.54 749.55L282.77 746.19L279 745.32L276.99 742.84L268.46 748.75L256.97 751.97L253.14 752.04L249.31 750.29L247.43 751.1V753.65L243.67 756.07L228.28 756.94L224.45 758.62L215.85 757.82L217.73 762.79L216.93 767.76L213.03 767.83L209.27 776.9L197.85 784.42L193.95 783.62L182.6 777.84L182.39 772.73L170.03 767.63L165.2 766.82L160.36 764.4L158.48 761.85V755.13L160.36 748.41V744.25L159.28 741.83L155.52 740.08L153.64 736.72V734.3L155.52 730.94L155.39 725.84L157.27 718.45L161.16 715.89L163.05 711.73L157.27 708.37L158.21 705.01L158.07 697.49L156.19 695.87L154.31 689.96L152.3 688.35L157.13 683.24L167.61 682.44L173.93 685.39L182.53 680.56L196.77 676.39L207.25 678.68L209.67 667.66L196.37 660.54L185.35 666.31L176.75 673.43L168.55 670.75L167.61 662.42L165.6 659.86L168.42 657.45L167.48 650.73L168.42 645.76L167.48 641.59L173.12 639.04L189.38 626.54L194.08 619.82V617.4L192.2 616.46L199.86 610.69L201.74 606.52L207.52 603.16L211.28 591.47L218 587.31L220.82 583.95L224.59 583.14L226.33 587.58L228.21 599.13L235.87 601.01L251.19 589.46L260.19 591.87L270.27 585.69L262.07 567.55L265.97 561.91L277.39 553.71L280.08 540.68L284.92 534.77L286.8 529.8L284.78 527.24L283.84 523.15L286.73 524.02L289.55 523.15L294.39 525.7L301.11 524.02L302.11 521.53L331.81 519.05L333.69 520.8L350.02 521.67L363.52 524.96L366.34 522.54L370.24 523.35L372.25 535.84V548.21L364.33 566.35L368.36 570.91L376.28 571.45V577.63L379.64 581.66L380.72 594.7L376.82 619.55L380.18 635.41L380.72 643.87L393.21 646.16L397.11 660.8L390.39 664.7L384.21 663.63L377.9 669.27L384.75 678.94L401.68 671.55L402.75 687.95L408.94 694.8L410.14 701.52L424.92 711.73L429.9 730.94V737.66L433.26 744.51L442.39 737.66L443.47 749.62L450.32 742.23L458.79 743.84L462.68 735.51L458.25 725.84L450.86 716.84L457.58 708.37H464.43L470.07 716.16L484.99 717.1L481.9 723.82L483.37 726.91L495.87 731.62L506.22 737.93L502.59 740.35L502.25 741.69L499.7 740.21L497.01 740.62L497.82 743.04L496.68 744.72L489.62 747.81L488.01 749.89L487.74 753.32L483.24 755L478.94 759.29L475.04 758.29L472.49 760.03L468.53 759.63L468.73 762.39L465.84 762.92L466.44 770.58L462.61 771.86L463.56 782.41L460.06 783.08L458.79 786.91L457.44 785.5L456.5 786.3L455.49 787.51L455.16 794.77L451.19 795.64L450.39 798.8L443.87 804.04L432.72 822.85L432.99 821.71L421.36 844.75V848.25L420.09 850.13L422.84 850.6L422.64 854.56L421.7 855.5L423.18 856.84L422.78 858.59L421.43 858.93L422.78 860.14L423.58 859.2L424.66 861.01L423.78 862.35L425.06 865.58L422.37 867.53L424.79 870.42L425.66 869.27L425.19 868.06H427.21L428.42 870.89L427.61 872.63L432.99 877.6L431.71 882.71L432.79 884.93L430.17 886.74L432.65 888.82L432.05 889.43L433.39 891.11L434.2 896.21L436.14 898.23L437.89 899.44L438.36 902.13L437.42 905.89L438.97 908.64L442.46 911.13L440.38 912.81L441.05 914.29L442.73 913.75L441.65 914.49L442.93 915.63L442.06 915.97L442.33 917.24L443.27 919.8L445.01 920.6L442.93 922.35L442.33 925.84L445.35 928.33L445.15 929.54L446.49 928.19L447.77 932.63L447.7 934.31L445.68 934.37L443.74 938.07L443.87 940.89L445.35 941.63L445.75 939.55L446.02 941.29L448.17 941.97V943.17L446.56 943.71L450.32 945.79L449.25 948.48L447.36 949.96L447.57 951.57L452.34 949.29L450.39 956.14L453.54 956.54L455.16 959.9L453.34 962.46L453.95 963.8L459.59 964.34L462.14 967.43V969.31H460.46L460.73 970.38L459.32 971.19L458.25 969.91L457.78 970.79L450.19 968.23Z"
						class="fill-maroon-flush-300 hover:fill-maroon-flush-500"
						stroke="black"
						stroke-width="2"
						mask="url(#path-2-inside-2_78_1665)"
					/>
					<mask id="path-3-inside-3_78_1665" fill="white">
						<path
							fill-rule="evenodd"
							clip-rule="evenodd"
							d="M412.16 266.24L408.53 283.03L409.61 299.76L405.78 310.24L409 313.27L409.67 315.48L408.4 317.9L410.14 329.05L409.14 334.03L411.76 341.28L411.15 352.3L408.06 368.63L410.01 377.83L407.86 388.58L412.43 391.13L413.77 402.02L415.52 404.57L411.62 407.93L412.56 413.71L423.04 418.81L425.06 428.82L424.12 433.86L428.89 438.03L427.07 446.36L426.27 463.96L427.21 470.54L426.34 480.69L423.45 479.81L421.57 480.62L415.79 478.13L422.57 489.02H426.4V490.7L421.7 493.92L423.58 499.83L420.76 506.55V513.2L424.72 527.45L429.56 532.48L420.09 548.21L421.9 554.18L420.09 556.67L422.98 560.03L423.98 567.02L421.16 571.18L411.62 572.79L402.96 581.13L401.95 576.15L398.12 572.79L396.24 568.56L390.53 565.14L389.59 563.52L391.47 559.36L397.11 554.39L399.06 549.42L398.99 545.25L397.11 544.31L396.17 538.53L392.27 535.17L384.62 530.94L382.73 525.09L380.85 524.29L379.78 519.18L376.96 518.38L373.06 523.35L366.34 522.54L363.52 524.96L350.02 521.67L333.69 520.8L331.81 519.05L302.11 521.53L301.11 524.02L294.39 525.7L289.55 523.15L286.73 524.02L283.84 523.15L282.5 499.57L278.6 489.49L276.65 487.81L278.53 483.71L277.53 479.54L278.47 476.19L276.58 471.21L279.41 459.52L278.33 458.72L279.27 450.39L272.42 441.12L274.3 431.17L272.29 423.65H270.34L266.57 426.13L261.8 422.84L256.03 423.65L254.15 418.61L256.97 416.93V415.18L255.09 414.38L256.03 411.96L253.07 406.85L253.21 403.49L248.5 395.03L245.95 385.62L241.78 379.58L242.19 373.4L240.44 371.65L238.83 367.35L230.63 359.29L233.72 354.99L232.51 344.1L234.66 336.71L234.06 328.72L231.91 325.09L222.03 315.01L221.63 310.51L223.24 294.52L222.1 293.78L225.19 293.92L228.21 295.66L232.24 294.93L233.32 295.53L232.31 298.89L235.13 301.04L242.52 301.58L266.44 308.63L267.11 309.84L269.33 309.3L269.8 307.35L273.76 308.36L275.11 307.02L284.65 307.09L286.73 305.94L289.62 306.15L293.58 308.63L298.69 306.82L299.9 304L302.85 302.92V301.44L299.23 299.76L297.95 297.21H300.37L300.97 295.53L300.23 294.79L302.11 295.26L303.39 294.46L304.13 295.66L305.61 294.79L305.74 295.6L306.95 295.33L306.28 296.47L311.45 298.08L314.48 295.53L315.42 296.27L317.16 294.72L318.37 295.66L323.55 291.5L324.28 292.24L329.32 289.01L328.58 288.07L330.47 286.8L331.54 283.71L329.73 272.62L327.04 266.91L335.24 254.48L333.62 245.08L335.3 239.63L341.69 241.31L344.04 232.31L343.16 229.76L339.2 228.08L340.14 223.78L337.05 215.99L335.64 215.11L336.71 213.84L335.97 212.9L337.32 211.55L337.99 212.96L339.07 212.16L343.23 206.31L346.05 205.1L346.99 205.77L347.66 202.75L349.55 204.3L350.08 207.12L350.35 212.76L348.81 215.38L348.87 218.2L353.38 222.57L353.58 224.59L355.32 224.72L354.65 225.73L356.26 227.47L355.79 229.15L357.27 229.56L357.81 231.1L357.74 234.13L360.97 245.95L365.8 252.4L367.82 252.47L369.36 249.71L372.66 249.51L375.34 253.68L375.14 256.03L380.72 256.36L382.33 257.57L385.69 257.24L386.76 259.99L388.98 261.2L390.12 263.42L391.94 263.15L392.88 261.74L394.09 263.15L395.7 261.67L397.85 264.49L398.79 263.75L400.34 264.89L401.14 263.55L402.15 264.83L407.79 264.02L412.16 266.24ZM285.72 309.37V309.3L285.45 309.44H285.65L285.72 309.37Z"
						/>
					</mask>
					<path
						fill-rule="evenodd"
						clip-rule="evenodd"
						d="M412.16 266.24L408.53 283.03L409.61 299.76L405.78 310.24L409 313.27L409.67 315.48L408.4 317.9L410.14 329.05L409.14 334.03L411.76 341.28L411.15 352.3L408.06 368.63L410.01 377.83L407.86 388.58L412.43 391.13L413.77 402.02L415.52 404.57L411.62 407.93L412.56 413.71L423.04 418.81L425.06 428.82L424.12 433.86L428.89 438.03L427.07 446.36L426.27 463.96L427.21 470.54L426.34 480.69L423.45 479.81L421.57 480.62L415.79 478.13L422.57 489.02H426.4V490.7L421.7 493.92L423.58 499.83L420.76 506.55V513.2L424.72 527.45L429.56 532.48L420.09 548.21L421.9 554.18L420.09 556.67L422.98 560.03L423.98 567.02L421.16 571.18L411.62 572.79L402.96 581.13L401.95 576.15L398.12 572.79L396.24 568.56L390.53 565.14L389.59 563.52L391.47 559.36L397.11 554.39L399.06 549.42L398.99 545.25L397.11 544.31L396.17 538.53L392.27 535.17L384.62 530.94L382.73 525.09L380.85 524.29L379.78 519.18L376.96 518.38L373.06 523.35L366.34 522.54L363.52 524.96L350.02 521.67L333.69 520.8L331.81 519.05L302.11 521.53L301.11 524.02L294.39 525.7L289.55 523.15L286.73 524.02L283.84 523.15L282.5 499.57L278.6 489.49L276.65 487.81L278.53 483.71L277.53 479.54L278.47 476.19L276.58 471.21L279.41 459.52L278.33 458.72L279.27 450.39L272.42 441.12L274.3 431.17L272.29 423.65H270.34L266.57 426.13L261.8 422.84L256.03 423.65L254.15 418.61L256.97 416.93V415.18L255.09 414.38L256.03 411.96L253.07 406.85L253.21 403.49L248.5 395.03L245.95 385.62L241.78 379.58L242.19 373.4L240.44 371.65L238.83 367.35L230.63 359.29L233.72 354.99L232.51 344.1L234.66 336.71L234.06 328.72L231.91 325.09L222.03 315.01L221.63 310.51L223.24 294.52L222.1 293.78L225.19 293.92L228.21 295.66L232.24 294.93L233.32 295.53L232.31 298.89L235.13 301.04L242.52 301.58L266.44 308.63L267.11 309.84L269.33 309.3L269.8 307.35L273.76 308.36L275.11 307.02L284.65 307.09L286.73 305.94L289.62 306.15L293.58 308.63L298.69 306.82L299.9 304L302.85 302.92V301.44L299.23 299.76L297.95 297.21H300.37L300.97 295.53L300.23 294.79L302.11 295.26L303.39 294.46L304.13 295.66L305.61 294.79L305.74 295.6L306.95 295.33L306.28 296.47L311.45 298.08L314.48 295.53L315.42 296.27L317.16 294.72L318.37 295.66L323.55 291.5L324.28 292.24L329.32 289.01L328.58 288.07L330.47 286.8L331.54 283.71L329.73 272.62L327.04 266.91L335.24 254.48L333.62 245.08L335.3 239.63L341.69 241.31L344.04 232.31L343.16 229.76L339.2 228.08L340.14 223.78L337.05 215.99L335.64 215.11L336.71 213.84L335.97 212.9L337.32 211.55L337.99 212.96L339.07 212.16L343.23 206.31L346.05 205.1L346.99 205.77L347.66 202.75L349.55 204.3L350.08 207.12L350.35 212.76L348.81 215.38L348.87 218.2L353.38 222.57L353.58 224.59L355.32 224.72L354.65 225.73L356.26 227.47L355.79 229.15L357.27 229.56L357.81 231.1L357.74 234.13L360.97 245.95L365.8 252.4L367.82 252.47L369.36 249.71L372.66 249.51L375.34 253.68L375.14 256.03L380.72 256.36L382.33 257.57L385.69 257.24L386.76 259.99L388.98 261.2L390.12 263.42L391.94 263.15L392.88 261.74L394.09 263.15L395.7 261.67L397.85 264.49L398.79 263.75L400.34 264.89L401.14 263.55L402.15 264.83L407.79 264.02L412.16 266.24ZM285.72 309.37V309.3L285.45 309.44H285.65L285.72 309.37Z"
						stroke="black"
						class="fill-maroon-flush-300 hover:fill-maroon-flush-500"
						stroke-width="2"
						mask="url(#path-3-inside-3_78_1665)"
					/>
					<mask id="path-4-inside-4_78_1665" fill="white">
						<path
							d="M760.57 550.76L757.21 547.6L752.78 546.32L751.37 544.71L748.41 545.59L747.27 544.51H743.98L738.47 546.06L734.91 552.1L734.24 555.6L738.67 564.87L738.54 566.75L735.51 568.76L735.04 571.65L733.7 573.06L732.22 576.89L732.62 581.26L722.28 592.88L718.04 593.49L714.08 592.28L714.42 588.92L711.53 587.44L712.2 583.34L710.92 579.92L712 576.29L715.42 573.94L716.3 571.32L714.35 568.83L714.62 567.55L713.61 566.95L711.73 560.84L709.71 559.96L708.91 557.34L702.66 556.67L697.69 553.85L696.75 555.8L692.04 556.13L691.24 550.22L688.89 549.35L686.6 545.59L687.81 543.64L687.41 539.2L688.82 537.25L688.28 535.64L684.65 534.23L682.24 534.7L689.49 532.48L690.84 527.11L686.8 523.89L681.43 523.35L680.09 520.12L680.35 516.9L682.24 513.41L680.35 506.42L679.55 484.79L678.47 481.29L677.94 469.47L679.01 467.99L679.28 459.93L671.62 432.92L667.05 426.34L665.57 415.32L662.35 406.45L659.26 403.9L652.54 405.78L645.82 404.43L641.79 402.02L635.61 401.61L634.67 396.91L638.43 389.79L639.78 384.01L638.16 380.52L634.27 377.02L634.4 370.98L652.81 365.2H659.26L662.48 357.14L654.42 348.27L656.03 338.59L660.07 332.15L670.55 336.18L675.38 328.92L677.8 318.44L681.83 311.99L693.12 304.73L691.51 295.87L692.31 287L684.25 280.55L681.83 270.07L701.18 262.01L708.44 251.66L719.72 248.3L714.89 239.43L711.66 228.28H700.38L692.31 221.02L688.28 208.93L666.52 200.87L656.84 195.23V184.75L651.2 183.94L640.72 185.55L635.88 176.68L628.89 156.39L624.19 148.6L622.85 142.82L625.4 115.28L628.09 107.75L629.83 107.35L632.45 108.9L635.61 108.29L639.91 105.34L641.19 102.51L642.8 103.72L643.61 102.18L645.42 103.05L650.66 101.44L652.81 101.84L654.62 100.43L652.68 98.62L653.75 98.15L652.47 97.74L653.15 96.2L654.96 93.65L658.79 91.23L658.18 89.82L660.94 86.46L663.36 85.92L661.68 83.43L661.88 81.28L662.15 79.54L664.43 77.45L664.5 74.16L672.09 74.77L677.26 73.22L682.71 76.45L684.32 76.18L685.19 74.57L685.12 72.82L686.2 72.28L684.12 72.01L684.86 69.8L684.12 68.59L685.06 67.71L684.12 66.23L682.71 66.3L683.04 64.82L681.83 64.15L683.04 60.86L680.76 58.17L681.23 55.55L679.82 55.15L680.96 53.13L680.22 51.32L678.81 50.85L679.08 46.68L677.13 46.75L677.73 44.87L678.88 45.61V44.2L677 44.13L676.26 42.52L678.27 41.24L675.18 36.2L675.99 34.12L674.24 29.82L675.85 29.35L673.7 26.93L674.91 22.23L677.53 18.67H679.35L675.72 15.65L677.47 14.57L678.14 15.31L678.88 13.56L677.13 11.95L676.73 8.32L680.22 6.58L679.28 5.3L679.95 4.09L681.36 5.3L683.92 4.22V2.68L685.53 3.08L689.16 1L693.39 4.56L692.78 7.85L693.66 8.66L695 7.72L696.88 8.19L699.64 10.27L702.12 9.4L706.96 13.56L708.17 18.8L715.42 21.29L717.57 18.67L720.66 19.61L721.47 22.83L727.79 24.04L727.85 21.09L730.07 23.57L731.62 28.68L733.56 30.63L727.38 37.28L726.44 42.59L727.92 50.38L730.61 53.13L731.28 57.23L744.98 66.64L745.66 69.19L744.65 78.26L749.15 84.44L750.23 92.57L753.99 94.45L754.39 97.14L756.14 98.75L753.99 102.98L755.6 106.01L752.51 108.96L752.78 112.99L750.09 116.49L715.69 192.27L771.99 190.66L772.26 192.14L770.25 195.63L772.13 199.79L771.72 202.62L773.87 204.16L772.66 207.05L775.49 208.53L774.81 210.61L783.48 210.01L780.73 215.45L782.74 217.93L785.03 216.46L787.04 219.28L790.8 221.43L790.94 222.23L787.85 222.5V223.58L791.07 226L790.87 228.88L794.03 231.37L794.16 233.25L792.42 234.73L794.63 235.6L794.97 237.42L793.42 248.17L795.64 249.78L797.39 258.38L799 261.07L798.6 262.81L795.91 263.01V265.37L793.22 266.64L793.56 272.62L795.1 273.7L793.22 275.98L793.49 281.89L795.51 283.77L795.64 284.65L793.96 285.59L795.91 287.94L793.22 293.51L795.3 293.45L792.95 296.81L793.69 304.47L789.53 307.69L792.42 308.36L792.55 309.71L790.13 310.51L789.86 312.93L786.5 313.33L785.56 314.81L788.86 320.32L786.77 321.19L787.85 325.36L786.97 326.1L785.5 325.23L784.49 327.04L785.97 333.22L783.68 336.44L787.18 338.73L785.43 340.95L788.79 347.06L788.25 347.73L785.97 347.06L785.7 347.93L792.68 356.94L793.76 366.68L791.54 368.16L792.89 370.04L791.34 370.98L790.4 373.53L789.46 373.33L789.06 376.35H787.38L786.1 378.5L782.74 379.78L783.14 385.96L781.87 386.23L782.74 388.31L781.73 396.24L783.28 397.85V403.76L788.45 409.41L792.95 410.82L794.83 412.56L793.96 414.24L795.1 419.01L794.3 423.25L792.89 422.78L789.8 424.05L788.79 432.65L786.64 433.32L787.18 437.89L785.16 438.16L785.7 440.91L787.91 441.72L789.06 447.16L786.64 448.44L787.44 450.25L780.86 452L777.1 451.26L774.68 449.45L770.92 450.12V447.03L768.83 446.15L766.08 449.18V451.73L764.33 455.49L758.42 458.58L756.67 466.11L762.18 473.36L761.85 476.52L764.6 478.94L765.34 482.84L761.31 483.91L760.17 482.9L758.56 483.91L753.72 482.16L746.93 484.05L749.69 494.33L752.58 514.28L752.85 523.35L751.7 535.31L753.05 542.09L758.29 546.59L760.57 550.76Z"
						/>
					</mask>
					<path
						d="M760.57 550.76L757.21 547.6L752.78 546.32L751.37 544.71L748.41 545.59L747.27 544.51H743.98L738.47 546.06L734.91 552.1L734.24 555.6L738.67 564.87L738.54 566.75L735.51 568.76L735.04 571.65L733.7 573.06L732.22 576.89L732.62 581.26L722.28 592.88L718.04 593.49L714.08 592.28L714.42 588.92L711.53 587.44L712.2 583.34L710.92 579.92L712 576.29L715.42 573.94L716.3 571.32L714.35 568.83L714.62 567.55L713.61 566.95L711.73 560.84L709.71 559.96L708.91 557.34L702.66 556.67L697.69 553.85L696.75 555.8L692.04 556.13L691.24 550.22L688.89 549.35L686.6 545.59L687.81 543.64L687.41 539.2L688.82 537.25L688.28 535.64L684.65 534.23L682.24 534.7L689.49 532.48L690.84 527.11L686.8 523.89L681.43 523.35L680.09 520.12L680.35 516.9L682.24 513.41L680.35 506.42L679.55 484.79L678.47 481.29L677.94 469.47L679.01 467.99L679.28 459.93L671.62 432.92L667.05 426.34L665.57 415.32L662.35 406.45L659.26 403.9L652.54 405.78L645.82 404.43L641.79 402.02L635.61 401.61L634.67 396.91L638.43 389.79L639.78 384.01L638.16 380.52L634.27 377.02L634.4 370.98L652.81 365.2H659.26L662.48 357.14L654.42 348.27L656.03 338.59L660.07 332.15L670.55 336.18L675.38 328.92L677.8 318.44L681.83 311.99L693.12 304.73L691.51 295.87L692.31 287L684.25 280.55L681.83 270.07L701.18 262.01L708.44 251.66L719.72 248.3L714.89 239.43L711.66 228.28H700.38L692.31 221.02L688.28 208.93L666.52 200.87L656.84 195.23V184.75L651.2 183.94L640.72 185.55L635.88 176.68L628.89 156.39L624.19 148.6L622.85 142.82L625.4 115.28L628.09 107.75L629.83 107.35L632.45 108.9L635.61 108.29L639.91 105.34L641.19 102.51L642.8 103.72L643.61 102.18L645.42 103.05L650.66 101.44L652.81 101.84L654.62 100.43L652.68 98.62L653.75 98.15L652.47 97.74L653.15 96.2L654.96 93.65L658.79 91.23L658.18 89.82L660.94 86.46L663.36 85.92L661.68 83.43L661.88 81.28L662.15 79.54L664.43 77.45L664.5 74.16L672.09 74.77L677.26 73.22L682.71 76.45L684.32 76.18L685.19 74.57L685.12 72.82L686.2 72.28L684.12 72.01L684.86 69.8L684.12 68.59L685.06 67.71L684.12 66.23L682.71 66.3L683.04 64.82L681.83 64.15L683.04 60.86L680.76 58.17L681.23 55.55L679.82 55.15L680.96 53.13L680.22 51.32L678.81 50.85L679.08 46.68L677.13 46.75L677.73 44.87L678.88 45.61V44.2L677 44.13L676.26 42.52L678.27 41.24L675.18 36.2L675.99 34.12L674.24 29.82L675.85 29.35L673.7 26.93L674.91 22.23L677.53 18.67H679.35L675.72 15.65L677.47 14.57L678.14 15.31L678.88 13.56L677.13 11.95L676.73 8.32L680.22 6.58L679.28 5.3L679.95 4.09L681.36 5.3L683.92 4.22V2.68L685.53 3.08L689.16 1L693.39 4.56L692.78 7.85L693.66 8.66L695 7.72L696.88 8.19L699.64 10.27L702.12 9.4L706.96 13.56L708.17 18.8L715.42 21.29L717.57 18.67L720.66 19.61L721.47 22.83L727.79 24.04L727.85 21.09L730.07 23.57L731.62 28.68L733.56 30.63L727.38 37.28L726.44 42.59L727.92 50.38L730.61 53.13L731.28 57.23L744.98 66.64L745.66 69.19L744.65 78.26L749.15 84.44L750.23 92.57L753.99 94.45L754.39 97.14L756.14 98.75L753.99 102.98L755.6 106.01L752.51 108.96L752.78 112.99L750.09 116.49L715.69 192.27L771.99 190.66L772.26 192.14L770.25 195.63L772.13 199.79L771.72 202.62L773.87 204.16L772.66 207.05L775.49 208.53L774.81 210.61L783.48 210.01L780.73 215.45L782.74 217.93L785.03 216.46L787.04 219.28L790.8 221.43L790.94 222.23L787.85 222.5V223.58L791.07 226L790.87 228.88L794.03 231.37L794.16 233.25L792.42 234.73L794.63 235.6L794.97 237.42L793.42 248.17L795.64 249.78L797.39 258.38L799 261.07L798.6 262.81L795.91 263.01V265.37L793.22 266.64L793.56 272.62L795.1 273.7L793.22 275.98L793.49 281.89L795.51 283.77L795.64 284.65L793.96 285.59L795.91 287.94L793.22 293.51L795.3 293.45L792.95 296.81L793.69 304.47L789.53 307.69L792.42 308.36L792.55 309.71L790.13 310.51L789.86 312.93L786.5 313.33L785.56 314.81L788.86 320.32L786.77 321.19L787.85 325.36L786.97 326.1L785.5 325.23L784.49 327.04L785.97 333.22L783.68 336.44L787.18 338.73L785.43 340.95L788.79 347.06L788.25 347.73L785.97 347.06L785.7 347.93L792.68 356.94L793.76 366.68L791.54 368.16L792.89 370.04L791.34 370.98L790.4 373.53L789.46 373.33L789.06 376.35H787.38L786.1 378.5L782.74 379.78L783.14 385.96L781.87 386.23L782.74 388.31L781.73 396.24L783.28 397.85V403.76L788.45 409.41L792.95 410.82L794.83 412.56L793.96 414.24L795.1 419.01L794.3 423.25L792.89 422.78L789.8 424.05L788.79 432.65L786.64 433.32L787.18 437.89L785.16 438.16L785.7 440.91L787.91 441.72L789.06 447.16L786.64 448.44L787.44 450.25L780.86 452L777.1 451.26L774.68 449.45L770.92 450.12V447.03L768.83 446.15L766.08 449.18V451.73L764.33 455.49L758.42 458.58L756.67 466.11L762.18 473.36L761.85 476.52L764.6 478.94L765.34 482.84L761.31 483.91L760.17 482.9L758.56 483.91L753.72 482.16L746.93 484.05L749.69 494.33L752.58 514.28L752.85 523.35L751.7 535.31L753.05 542.09L758.29 546.59L760.57 550.76Z"
						stroke="black"
						class="fill-maroon-flush-300 hover:fill-maroon-flush-500"
						stroke-width="2"
						mask="url(#path-4-inside-4_78_1665)"
					/>
					<mask id="path-5-inside-5_78_1665" fill="white">
						<path
							fill-rule="evenodd"
							clip-rule="evenodd"
							d="M50.72 534.63L57.97 554.25L67.11 549.95L86.59 564.73L100.97 549.01L107.15 560.97L113.87 557.61L116.69 548.47L124.35 533.69L133.35 534.63L141.01 542.29L149.61 545.65L156.33 541.35L161.57 527.11L169.23 529.39L180.65 530.87L188.17 528.99L196.37 537.05L217.33 543.77L233.05 540.95L251.59 531.81L261.13 525.23L269.73 526.57L277.39 517.97L282.63 509.51L283.84 523.08L284.78 527.24L286.8 529.8L284.92 534.77L280.08 540.68L277.39 553.71L265.97 561.91L262.07 567.55L270.27 585.69L260.19 591.87L251.19 589.46L235.87 601.01L228.21 599.13L226.33 587.58L224.59 583.14L220.82 583.95L218 587.31L211.28 591.47L207.52 603.16L201.74 606.52L199.86 610.69L192.2 616.46L194.08 617.4V619.82L189.38 626.54L173.12 639.04L167.48 641.59L168.42 645.76L167.48 650.73L168.42 657.45L165.6 659.86L167.61 662.42L168.55 670.75L176.75 673.43L185.35 666.31L196.37 660.54L209.67 667.66L207.25 678.68L196.77 676.39L182.53 680.56L173.93 685.39L167.61 682.44L157.13 683.24L152.3 688.35L154.31 689.96L156.19 695.87L158.07 697.49L158.21 705.01L157.27 708.37L163.05 711.73L161.16 715.89L157.27 718.45L155.39 725.84L155.52 730.94L153.64 734.3V736.72L155.52 740.08L159.28 741.83L160.36 744.25V748.41L158.48 755.13V761.85L160.36 764.4L165.2 766.82L170.03 767.63L182.39 772.73L183.4 781.87L179.71 783.62L176.75 787.78H173.93L173.86 789.46L168.15 793.56H165.33L162.44 795.3L163.45 806.99L160.63 811.97V814.52L156.86 815.39L154.98 817.74L150.21 828.63V831.25L139.8 837.03V838.71L134.96 842.87L128.38 846.23L120.65 847.04L116.82 846.23L113.73 847.51L113.2 845.69L117.56 842L109.97 839.51L106.75 836.29L108.76 832.26L112.05 830.31L108.76 820.63L99.76 820.9L95.53 817.48L99.76 802.49L105.81 800.81L109.57 801.42L109.77 794.57L110.78 793.69L114.41 794.36L115.82 789.59L113.53 789.73L102.98 795.3L96.33 795.91L98.89 788.86L93.04 787.51L91.76 782.14L98.21 781.53L98.55 779.79L97.88 777.97L94.65 779.32L92.37 778.17L88.74 778.44L86.52 752.91L77.79 746.8L82.63 742.77L73.09 734.84L72.62 730.94L69.8 726.71L71.07 723.82L71 721.54L69.33 719.52L70.27 708.37L68.32 702.19L59.58 703L60.19 698.83L58.31 698.16L59.05 694.4L50.92 697.42L47.22 695.94L50.92 686.33L40.44 687.48L35.67 682.1L40.64 666.65L43.93 665.24L43.86 663.36L39.97 665.1L38.76 665.17L37.61 663.56L31.43 663.89L31.9 653.62L26.6 646.43V643.47L18.53 638.16L20.42 633.93L19.74 632.99L14.17 633.39L9.94 631.71L9.73 629.3L10.81 627.68L8.05 620.83L8.93 619.02L6.98 613.78L7.45 608.94L8.93 607.39L7.38 600.61L9.2 591.87L5.9 581.93L5.84 580.92L8.66 583.21L9.2 580.99L11.61 584.62L16.12 586.63L18.67 589.46L19.07 588.38L19.27 589.59L20.21 589.05L22.9 590.53L23.64 588.31L25.19 590.4L30.43 591.81L28.95 596.85L34.79 597.12L34.93 595.03L38.22 594.56L36.88 592.14H38.62L38.49 591.47L36.14 590.8L37.61 589.25L36.74 586.16L38.49 574.81L37.35 574.61L40.91 570.31L37.61 570.98L32.17 566.48L31.03 568.02L3.96 568.43L2.68 557.54L1 553.45L6.98 534.84L5.9 534.5L6.31 532.96L7.52 533.22L12.22 528.45L15.04 527.85L16.65 526.37L26.93 526.84L35.26 525.63L44.8 527.65L46.68 531.95L50.72 534.63ZM9.33 585.09L9.06 584.75L9.67 585.56L9.33 585.09ZM8.79 584.01L8.86 584.08L8.79 583.81V584.01Z"
						/>
					</mask>
					<path
						fill-rule="evenodd"
						clip-rule="evenodd"
						d="M50.72 534.63L57.97 554.25L67.11 549.95L86.59 564.73L100.97 549.01L107.15 560.97L113.87 557.61L116.69 548.47L124.35 533.69L133.35 534.63L141.01 542.29L149.61 545.65L156.33 541.35L161.57 527.11L169.23 529.39L180.65 530.87L188.17 528.99L196.37 537.05L217.33 543.77L233.05 540.95L251.59 531.81L261.13 525.23L269.73 526.57L277.39 517.97L282.63 509.51L283.84 523.08L284.78 527.24L286.8 529.8L284.92 534.77L280.08 540.68L277.39 553.71L265.97 561.91L262.07 567.55L270.27 585.69L260.19 591.87L251.19 589.46L235.87 601.01L228.21 599.13L226.33 587.58L224.59 583.14L220.82 583.95L218 587.31L211.28 591.47L207.52 603.16L201.74 606.52L199.86 610.69L192.2 616.46L194.08 617.4V619.82L189.38 626.54L173.12 639.04L167.48 641.59L168.42 645.76L167.48 650.73L168.42 657.45L165.6 659.86L167.61 662.42L168.55 670.75L176.75 673.43L185.35 666.31L196.37 660.54L209.67 667.66L207.25 678.68L196.77 676.39L182.53 680.56L173.93 685.39L167.61 682.44L157.13 683.24L152.3 688.35L154.31 689.96L156.19 695.87L158.07 697.49L158.21 705.01L157.27 708.37L163.05 711.73L161.16 715.89L157.27 718.45L155.39 725.84L155.52 730.94L153.64 734.3V736.72L155.52 740.08L159.28 741.83L160.36 744.25V748.41L158.48 755.13V761.85L160.36 764.4L165.2 766.82L170.03 767.63L182.39 772.73L183.4 781.87L179.71 783.62L176.75 787.78H173.93L173.86 789.46L168.15 793.56H165.33L162.44 795.3L163.45 806.99L160.63 811.97V814.52L156.86 815.39L154.98 817.74L150.21 828.63V831.25L139.8 837.03V838.71L134.96 842.87L128.38 846.23L120.65 847.04L116.82 846.23L113.73 847.51L113.2 845.69L117.56 842L109.97 839.51L106.75 836.29L108.76 832.26L112.05 830.31L108.76 820.63L99.76 820.9L95.53 817.48L99.76 802.49L105.81 800.81L109.57 801.42L109.77 794.57L110.78 793.69L114.41 794.36L115.82 789.59L113.53 789.73L102.98 795.3L96.33 795.91L98.89 788.86L93.04 787.51L91.76 782.14L98.21 781.53L98.55 779.79L97.88 777.97L94.65 779.32L92.37 778.17L88.74 778.44L86.52 752.91L77.79 746.8L82.63 742.77L73.09 734.84L72.62 730.94L69.8 726.71L71.07 723.82L71 721.54L69.33 719.52L70.27 708.37L68.32 702.19L59.58 703L60.19 698.83L58.31 698.16L59.05 694.4L50.92 697.42L47.22 695.94L50.92 686.33L40.44 687.48L35.67 682.1L40.64 666.65L43.93 665.24L43.86 663.36L39.97 665.1L38.76 665.17L37.61 663.56L31.43 663.89L31.9 653.62L26.6 646.43V643.47L18.53 638.16L20.42 633.93L19.74 632.99L14.17 633.39L9.94 631.71L9.73 629.3L10.81 627.68L8.05 620.83L8.93 619.02L6.98 613.78L7.45 608.94L8.93 607.39L7.38 600.61L9.2 591.87L5.9 581.93L5.84 580.92L8.66 583.21L9.2 580.99L11.61 584.62L16.12 586.63L18.67 589.46L19.07 588.38L19.27 589.59L20.21 589.05L22.9 590.53L23.64 588.31L25.19 590.4L30.43 591.81L28.95 596.85L34.79 597.12L34.93 595.03L38.22 594.56L36.88 592.14H38.62L38.49 591.47L36.14 590.8L37.61 589.25L36.74 586.16L38.49 574.81L37.35 574.61L40.91 570.31L37.61 570.98L32.17 566.48L31.03 568.02L3.96 568.43L2.68 557.54L1 553.45L6.98 534.84L5.9 534.5L6.31 532.96L7.52 533.22L12.22 528.45L15.04 527.85L16.65 526.37L26.93 526.84L35.26 525.63L44.8 527.65L46.68 531.95L50.72 534.63ZM9.33 585.09L9.06 584.75L9.67 585.56L9.33 585.09ZM8.79 584.01L8.86 584.08L8.79 583.81V584.01Z"
						stroke="black"
						class="fill-maroon-flush-300 hover:fill-maroon-flush-500"
						stroke-width="2"
						mask="url(#path-5-inside-5_78_1665)"
					/>
					<mask id="path-6-inside-6_78_1665" fill="white">
						<path
							fill-rule="evenodd"
							clip-rule="evenodd"
							d="M106.75 836.29L109.97 839.51L117.56 842L113.2 845.69L113.73 847.51L116.82 846.23L120.65 847.04L128.38 846.23L134.96 842.87L139.8 838.71V837.03L150.21 831.25V828.63L154.98 817.74L156.86 815.39L160.63 814.52V811.97L163.45 806.99L162.44 795.3L165.33 793.56H168.15L173.86 789.46L173.93 787.78H176.75L178.77 786.03L179.71 783.62L183.4 781.87L182.46 777.77L193.95 783.62L197.85 784.42L209.27 776.9L213.03 767.83L216.93 767.76L217.73 762.79L215.85 757.82L224.45 758.62L228.28 756.94L243.67 756.07L247.43 753.65V751.1L249.31 750.29L253.14 752.04L256.97 751.97L268.46 748.75L276.99 742.84L279 745.32L282.77 746.19L288.54 749.55L290.42 753.72L290.49 757.95L293.31 758.76L299.16 762.92L303.86 757.95L310.58 756.34L314.34 749.62L320.12 745.46L323.95 750.49L325.9 756.34L323.01 758.89L324.96 763.86V772.19L330.73 771.39L333.69 784.69L337.45 788.12L339.47 794.77L346.99 788.99L365.13 784.02L367.08 785.7L365.27 789.93L366.14 791.54L368.02 789.06H369.97L370.91 793.22L369.03 796.51L372.93 803.23L386.36 817.48L388.24 816.67L392.01 817.54L392.95 821.64L388.24 830.91L389.18 836.76L399.4 847.44L406.79 860.61L411.22 876.33L410.28 885.6L423.04 899.57L424.79 909.11L433.93 919.19L435.67 926.18L430.84 934.11L409.47 931.42L422.1 947.68L428.28 945.53L437.96 957.75L450.19 968.23L459.99 971.46L453.54 973.34L454.62 975.42L451.53 977.84L450.52 975.76L448.17 977.37L449.85 978.45L450.25 980.53L448.91 981.33L450.59 982.61L448.98 983.22L447.1 982.14L447.57 984.09L446.02 984.76L446.56 986.98L442.26 986.51L442.33 989.13L437.69 987.85L434.26 989.67L434.33 985.23L431.44 985.3L431.24 983.35L430.23 984.56L430.84 986.37L428.82 985.57L428.02 983.48L421.16 984.76L420.49 986.98L424.59 991.75L423.25 993.29L425.6 994.23L429.36 998.74L429.56 1007L428.28 1010.29L425.13 1010.49L424.86 1012.31L421.3 1013.45L420.02 1010.83L420.89 1006.6L418.95 1006.86L419.42 1009.28L416.86 1008.48L412.09 1011.43L412.36 1013.92L409.74 1015.13L410.14 1018.22L405.44 1024.8L401.81 1027.36L397.45 1028.5L389.99 1033.67L388.31 1038.78L386.83 1038.51L383.27 1040.52L379.85 1039.11L378.5 1039.65V1043.21L376.96 1043.68L372.59 1039.11L366.81 1039.38L365.47 1040.46L365 1042.94L358.82 1046.77L356.4 1044.42L350.49 1047.04L347.46 1043.88L345.45 1045.49L342.69 1043.75L341.75 1044.49L342.89 1046.17L341.15 1047.24L338.39 1047.11L337.52 1043.21L334.36 1041.6L334.63 1047.17L331.27 1048.38L331.14 1051.41L327.85 1057.59L324.89 1059L322.34 1058.33L323.48 1060.54L319.65 1065.52L321.06 1069.08L317.3 1072.91L315.48 1072.5L315.28 1069.08L312.46 1067.06L312.59 1065.38L314.95 1065.65L314.54 1064.1L313.07 1063.5L308.7 1065.04L309.91 1060.81L305.54 1062.89L304.13 1062.16L305.2 1059.07L309.3 1055.64L307.42 1054.3L307.96 1050.4L303.73 1051.94L302.11 1051.41L302.38 1047.91L299.36 1049.93L297.48 1046.97L288.34 1054.83L287.13 1052.55L275.17 1045.96L275.04 1036.42L268.66 1035.35L265.23 1031.79L267.92 1019.97L266.37 1019.56L267.04 1018.55H262.48L270.54 1005.72L257.17 1005.79L260.46 996.52L255.96 995.58L256.56 994.3H253.47L254.08 991.21L260.46 988.93L253.54 975.83L256.83 973.88L256.77 970.05L249.44 968.23L251.06 962.79L244.27 961.52L244.94 955.4L250.38 954.6L249.64 952.38L247.02 952.45L246.29 949.15L247.43 948.28L239.23 946L238.83 943.85L245.21 939.41L239.7 937.2L237.82 935.38L235.87 935.72L236.01 934.91L233.18 932.69L241.58 927.86L232.92 929.2L230.63 925.57L233.25 922.68L235.47 916.17L231.57 915.97L231.17 912.2L234.93 910.73L241.25 910.59L241.72 908.44L237.42 907.03L238.22 906.09L225.93 905.22L224.32 906.69L219.41 904.75L220.96 901.79L217.06 899.51L224.92 898.16L226.26 890.97L222.64 886.47L212.76 889.03L210.41 887.55L208.93 888.22L208.66 886.61L203.49 884.05L205.3 881.57L216.72 878.54L210.07 868.74L207.05 869.21L204.3 868L204.36 867.26L202.15 867.73L205.77 859.33L187.3 858.05L185.48 860.27L184.21 858.79L183.74 855.64L181.92 859.87H181.86L182.13 857.99L179.91 854.56L181.25 853.82L180.24 850.46L181.72 850.4L182.66 847.91L181.45 845.96L180.71 846.3L181.45 845.22L179.98 843.88L180.04 841.53L178.77 842.47L175.47 839.91L177.09 859.73L174.74 859.46V861.21L180.11 867.06L174.47 868.47L171.58 871.89L173.93 876.26L172.25 879.62L166.74 881.5L167.48 885.06L164.59 885.93L163.05 885.33L156.6 891.44L161.3 891.85L159.82 902.6L156.73 902.8L156.06 907.57H158.14L157.33 913.88L163.05 913.35L164.79 918.92L163.38 925.71L163.85 929.07L166.74 932.49L166.94 937.53H168.62L170.37 940.76L172.12 952.31L176.28 959.84L174.94 967.97L177.89 967.9L178.3 968.7L177.83 975.56L181.25 975.83L180.31 980.06L178.5 980.8L178.36 984.76L176.82 987.11L181.12 987.78L180.71 988.52L184.34 991.82L181.45 994.23L177.96 995.24L177.15 990.14L173.79 991.88L169.02 992.22L168.69 993.56L166.74 993.83L149.21 984.22L133.89 962.73L134.36 951.71L130.46 952.31L130.39 944.99L127.24 943.44L124.62 928.8L118.03 925.3L118.97 918.18L118.23 871.96L115.08 870.35L114.88 866.59L119.44 865.44L120.18 862.02L114.47 861.61L108.9 845.83L112.93 843.74L113.53 842.13L103.92 839.11L102.51 835.01L107.22 830.11L109.9 831.18L106.75 836.29ZM162.71 912.54L162.1 911.73L162.04 911.06H162.1L162.71 912.54Z"
						/>
					</mask>
					<path
						fill-rule="evenodd"
						clip-rule="evenodd"
						d="M106.75 836.29L109.97 839.51L117.56 842L113.2 845.69L113.73 847.51L116.82 846.23L120.65 847.04L128.38 846.23L134.96 842.87L139.8 838.71V837.03L150.21 831.25V828.63L154.98 817.74L156.86 815.39L160.63 814.52V811.97L163.45 806.99L162.44 795.3L165.33 793.56H168.15L173.86 789.46L173.93 787.78H176.75L178.77 786.03L179.71 783.62L183.4 781.87L182.46 777.77L193.95 783.62L197.85 784.42L209.27 776.9L213.03 767.83L216.93 767.76L217.73 762.79L215.85 757.82L224.45 758.62L228.28 756.94L243.67 756.07L247.43 753.65V751.1L249.31 750.29L253.14 752.04L256.97 751.97L268.46 748.75L276.99 742.84L279 745.32L282.77 746.19L288.54 749.55L290.42 753.72L290.49 757.95L293.31 758.76L299.16 762.92L303.86 757.95L310.58 756.34L314.34 749.62L320.12 745.46L323.95 750.49L325.9 756.34L323.01 758.89L324.96 763.86V772.19L330.73 771.39L333.69 784.69L337.45 788.12L339.47 794.77L346.99 788.99L365.13 784.02L367.08 785.7L365.27 789.93L366.14 791.54L368.02 789.06H369.97L370.91 793.22L369.03 796.51L372.93 803.23L386.36 817.48L388.24 816.67L392.01 817.54L392.95 821.64L388.24 830.91L389.18 836.76L399.4 847.44L406.79 860.61L411.22 876.33L410.28 885.6L423.04 899.57L424.79 909.11L433.93 919.19L435.67 926.18L430.84 934.11L409.47 931.42L422.1 947.68L428.28 945.53L437.96 957.75L450.19 968.23L459.99 971.46L453.54 973.34L454.62 975.42L451.53 977.84L450.52 975.76L448.17 977.37L449.85 978.45L450.25 980.53L448.91 981.33L450.59 982.61L448.98 983.22L447.1 982.14L447.57 984.09L446.02 984.76L446.56 986.98L442.26 986.51L442.33 989.13L437.69 987.85L434.26 989.67L434.33 985.23L431.44 985.3L431.24 983.35L430.23 984.56L430.84 986.37L428.82 985.57L428.02 983.48L421.16 984.76L420.49 986.98L424.59 991.75L423.25 993.29L425.6 994.23L429.36 998.74L429.56 1007L428.28 1010.29L425.13 1010.49L424.86 1012.31L421.3 1013.45L420.02 1010.83L420.89 1006.6L418.95 1006.86L419.42 1009.28L416.86 1008.48L412.09 1011.43L412.36 1013.92L409.74 1015.13L410.14 1018.22L405.44 1024.8L401.81 1027.36L397.45 1028.5L389.99 1033.67L388.31 1038.78L386.83 1038.51L383.27 1040.52L379.85 1039.11L378.5 1039.65V1043.21L376.96 1043.68L372.59 1039.11L366.81 1039.38L365.47 1040.46L365 1042.94L358.82 1046.77L356.4 1044.42L350.49 1047.04L347.46 1043.88L345.45 1045.49L342.69 1043.75L341.75 1044.49L342.89 1046.17L341.15 1047.24L338.39 1047.11L337.52 1043.21L334.36 1041.6L334.63 1047.17L331.27 1048.38L331.14 1051.41L327.85 1057.59L324.89 1059L322.34 1058.33L323.48 1060.54L319.65 1065.52L321.06 1069.08L317.3 1072.91L315.48 1072.5L315.28 1069.08L312.46 1067.06L312.59 1065.38L314.95 1065.65L314.54 1064.1L313.07 1063.5L308.7 1065.04L309.91 1060.81L305.54 1062.89L304.13 1062.16L305.2 1059.07L309.3 1055.64L307.42 1054.3L307.96 1050.4L303.73 1051.94L302.11 1051.41L302.38 1047.91L299.36 1049.93L297.48 1046.97L288.34 1054.83L287.13 1052.55L275.17 1045.96L275.04 1036.42L268.66 1035.35L265.23 1031.79L267.92 1019.97L266.37 1019.56L267.04 1018.55H262.48L270.54 1005.72L257.17 1005.79L260.46 996.52L255.96 995.58L256.56 994.3H253.47L254.08 991.21L260.46 988.93L253.54 975.83L256.83 973.88L256.77 970.05L249.44 968.23L251.06 962.79L244.27 961.52L244.94 955.4L250.38 954.6L249.64 952.38L247.02 952.45L246.29 949.15L247.43 948.28L239.23 946L238.83 943.85L245.21 939.41L239.7 937.2L237.82 935.38L235.87 935.72L236.01 934.91L233.18 932.69L241.58 927.86L232.92 929.2L230.63 925.57L233.25 922.68L235.47 916.17L231.57 915.97L231.17 912.2L234.93 910.73L241.25 910.59L241.72 908.44L237.42 907.03L238.22 906.09L225.93 905.22L224.32 906.69L219.41 904.75L220.96 901.79L217.06 899.51L224.92 898.16L226.26 890.97L222.64 886.47L212.76 889.03L210.41 887.55L208.93 888.22L208.66 886.61L203.49 884.05L205.3 881.57L216.72 878.54L210.07 868.74L207.05 869.21L204.3 868L204.36 867.26L202.15 867.73L205.77 859.33L187.3 858.05L185.48 860.27L184.21 858.79L183.74 855.64L181.92 859.87H181.86L182.13 857.99L179.91 854.56L181.25 853.82L180.24 850.46L181.72 850.4L182.66 847.91L181.45 845.96L180.71 846.3L181.45 845.22L179.98 843.88L180.04 841.53L178.77 842.47L175.47 839.91L177.09 859.73L174.74 859.46V861.21L180.11 867.06L174.47 868.47L171.58 871.89L173.93 876.26L172.25 879.62L166.74 881.5L167.48 885.06L164.59 885.93L163.05 885.33L156.6 891.44L161.3 891.85L159.82 902.6L156.73 902.8L156.06 907.57H158.14L157.33 913.88L163.05 913.35L164.79 918.92L163.38 925.71L163.85 929.07L166.74 932.49L166.94 937.53H168.62L170.37 940.76L172.12 952.31L176.28 959.84L174.94 967.97L177.89 967.9L178.3 968.7L177.83 975.56L181.25 975.83L180.31 980.06L178.5 980.8L178.36 984.76L176.82 987.11L181.12 987.78L180.71 988.52L184.34 991.82L181.45 994.23L177.96 995.24L177.15 990.14L173.79 991.88L169.02 992.22L168.69 993.56L166.74 993.83L149.21 984.22L133.89 962.73L134.36 951.71L130.46 952.31L130.39 944.99L127.24 943.44L124.62 928.8L118.03 925.3L118.97 918.18L118.23 871.96L115.08 870.35L114.88 866.59L119.44 865.44L120.18 862.02L114.47 861.61L108.9 845.83L112.93 843.74L113.53 842.13L103.92 839.11L102.51 835.01L107.22 830.11L109.9 831.18L106.75 836.29ZM162.71 912.54L162.1 911.73L162.04 911.06H162.1L162.71 912.54Z"
						stroke="black"
						class="fill-maroon-flush-300 hover:fill-maroon-flush-500"
						stroke-width="2"
						mask="url(#path-6-inside-6_78_1665)"
					/>
					<mask id="path-7-inside-7_78_1665" fill="white">
						<path
							d="M506.96 267.65L509.31 266.51L509.51 262.34L512.26 261.33L513 259.52L511.93 258.51L513.07 256.5L515.22 256.43L514.01 255.83L515.02 255.42L514.21 255.09L514.95 252.6L513.88 251.66L514.82 250.72L513.07 249.51L515.49 247.76L513.07 246.69L532.82 179.57L518.85 133.01L520.46 134.16L522.94 133.62L523.68 131.87L527.11 130.39L528.99 131.4L532.55 128.98L534.57 125.22L536.52 124.89L536.85 123.94L539.14 124.01L543.57 120.05L548.68 124.35L551.77 124.42L549.68 126.77L553.11 129.19L553.92 133.69L555.8 136.98L561.17 137.31L563.32 140.74L569.91 143.29L570.24 140.27L569.23 137.38L570.17 132.61L567.96 131.34L567.29 128.98L565.4 128.78L563.19 124.62L557.95 119.58L558.96 117.5L562.31 117.09L558.08 113.33L558.48 111.38L557.54 109.23L555.06 110.64L552.44 107.89L554.32 106.34L553.98 104.66L550.42 104.6L553.78 101.17L560.3 103.66L561.58 106.21L563.05 106.48L563.32 100.77L565.87 98.4201L567.35 98.9501L565.61 97.8101L566.14 97.2701L568.23 98.8901L569.7 98.5501L570.11 97.2701L569.1 96.2001L570.31 95.1201L577.16 99.8301V102.45L579.45 103.12L586.1 99.9601L588.52 100.63L587.1 102.18L589.25 102.04L590.6 104.6L596.71 104.26L599.33 106.61L601.48 106.01L602.62 107.15L605.38 106.01L610.48 107.08L628.09 107.75L625.4 115.28L622.85 142.82L624.19 148.6L628.89 156.39L635.88 176.68L640.72 185.55L651.2 183.94L656.84 184.75V195.23L666.52 200.87L688.28 208.93L692.31 221.02L700.38 228.28H711.66L714.89 239.43L719.72 248.3L708.44 251.66L701.18 262.01L681.83 270.07L684.25 280.55L692.31 287L691.51 295.87L693.12 304.73L681.83 311.99L677.8 318.44L675.38 328.92L670.55 336.18L660.07 332.15L656.03 338.59L654.42 348.27L662.48 357.14L659.26 365.2H652.81L634.4 370.98L626.88 369.23L622.71 365.06L616.53 364.26L610.35 365.87L608.07 361.97V356.33L604.44 350.55L605.11 342.89L615.99 339L618.68 330.4L613.17 320.32L612.77 290.09L585.36 296.27L577.43 297.08L573.8 300.7L558.62 310.51L552.84 311.05L539.54 299.23L526.77 294.66L513.74 284.98L515.08 282.43L514.55 279.61L506.96 267.65Z"
						/>
					</mask>
					<path
						d="M506.96 267.65L509.31 266.51L509.51 262.34L512.26 261.33L513 259.52L511.93 258.51L513.07 256.5L515.22 256.43L514.01 255.83L515.02 255.42L514.21 255.09L514.95 252.6L513.88 251.66L514.82 250.72L513.07 249.51L515.49 247.76L513.07 246.69L532.82 179.57L518.85 133.01L520.46 134.16L522.94 133.62L523.68 131.87L527.11 130.39L528.99 131.4L532.55 128.98L534.57 125.22L536.52 124.89L536.85 123.94L539.14 124.01L543.57 120.05L548.68 124.35L551.77 124.42L549.68 126.77L553.11 129.19L553.92 133.69L555.8 136.98L561.17 137.31L563.32 140.74L569.91 143.29L570.24 140.27L569.23 137.38L570.17 132.61L567.96 131.34L567.29 128.98L565.4 128.78L563.19 124.62L557.95 119.58L558.96 117.5L562.31 117.09L558.08 113.33L558.48 111.38L557.54 109.23L555.06 110.64L552.44 107.89L554.32 106.34L553.98 104.66L550.42 104.6L553.78 101.17L560.3 103.66L561.58 106.21L563.05 106.48L563.32 100.77L565.87 98.4201L567.35 98.9501L565.61 97.8101L566.14 97.2701L568.23 98.8901L569.7 98.5501L570.11 97.2701L569.1 96.2001L570.31 95.1201L577.16 99.8301V102.45L579.45 103.12L586.1 99.9601L588.52 100.63L587.1 102.18L589.25 102.04L590.6 104.6L596.71 104.26L599.33 106.61L601.48 106.01L602.62 107.15L605.38 106.01L610.48 107.08L628.09 107.75L625.4 115.28L622.85 142.82L624.19 148.6L628.89 156.39L635.88 176.68L640.72 185.55L651.2 183.94L656.84 184.75V195.23L666.52 200.87L688.28 208.93L692.31 221.02L700.38 228.28H711.66L714.89 239.43L719.72 248.3L708.44 251.66L701.18 262.01L681.83 270.07L684.25 280.55L692.31 287L691.51 295.87L693.12 304.73L681.83 311.99L677.8 318.44L675.38 328.92L670.55 336.18L660.07 332.15L656.03 338.59L654.42 348.27L662.48 357.14L659.26 365.2H652.81L634.4 370.98L626.88 369.23L622.71 365.06L616.53 364.26L610.35 365.87L608.07 361.97V356.33L604.44 350.55L605.11 342.89L615.99 339L618.68 330.4L613.17 320.32L612.77 290.09L585.36 296.27L577.43 297.08L573.8 300.7L558.62 310.51L552.84 311.05L539.54 299.23L526.77 294.66L513.74 284.98L515.08 282.43L514.55 279.61L506.96 267.65Z"
						stroke="black"
						class="fill-maroon-flush-300 hover:fill-maroon-flush-500"
						stroke-width="2"
						mask="url(#path-7-inside-7_78_1665)"
					/>
					<mask id="path-8-inside-8_78_1665" fill="white">
						<path
							d="M223.24 294.52L221.63 310.51L222.03 315.01L231.91 325.09L234.06 328.72L234.66 336.71L232.51 344.1L233.72 354.99L230.63 359.29L238.83 367.35L240.44 371.65L242.19 373.4L241.78 379.58L245.95 385.62L248.5 395.03L253.21 403.49L253.07 406.85L256.03 411.96L255.09 414.38L256.97 415.18V416.93L254.15 418.61L256.03 423.65L261.8 422.84L266.57 426.13L270.34 423.65H272.29L274.3 431.17L272.42 441.12L279.27 450.39L278.33 458.72L279.41 459.52L276.58 471.21L278.47 476.19L277.53 479.54L278.53 483.71L276.65 487.81L278.6 489.49L282.5 499.57L282.63 509.51L277.39 517.97L269.73 526.57L261.13 525.23L251.59 531.81L233.05 540.95L217.33 543.77L196.37 537.05L188.17 528.99L180.65 530.87L169.23 529.39L161.57 527.11L156.33 541.35L149.61 545.65L141.01 542.29L133.35 534.63L124.35 533.69L116.69 548.47L113.87 557.61L107.15 560.97L100.97 549.01L86.59 564.73L67.11 549.95L57.97 554.25L50.72 534.63L48.97 533.83L52.87 526.84L52.13 523.21L55.75 517.57L55.69 504.54L54.21 503.73L54.34 501.58L52.93 500.1L56.36 495.27L57.84 486.73L60.39 484.92L64.02 478.6L71.47 469.13L70.6 466.51L67.98 459.86L62.61 452.6L59.18 441.92L56.56 441.59L55.02 439.91L54.28 427.75L65.29 422.17L66.17 418.07L63.01 411.62L57.37 408.73L59.72 406.99L85.79 409.2L84.11 401.55L78.13 397.11L83.23 384.62L91.43 371.11L93.11 371.78L92.03 374.94L94.12 377.16L94.05 381.12L102.04 378.1L100.5 375.61L104.66 367.82L103.25 363.86L105 361.03L105.81 362.85L112.39 366.07L118.17 363.39L120.38 365.33L123.34 365.06L129.66 371.72L134.29 370.31L137.78 371.92L143.76 368.89L153.1 374.87L154.92 375.21L155.86 373.73L154.58 373.13L154.71 369.83L153.51 368.63L154.18 364.26L152.23 363.05L153.57 362.85L151.89 361.24L152.9 360.16L152.03 359.02L152.7 358.21L151.62 357.88L163.38 342.36L167.14 331.2L167.21 326.3L154.18 306.01L152.43 287.27L154.78 286.19L167.01 286.39L170.57 284.78L170.44 285.99L172.05 286.39L177.96 285.79L186.76 287.87L188.44 286.8L190.05 287.47L190.99 291.16L193.14 291.9L194.49 290.69L196.91 290.49L199.19 293.92L202.82 291.5L204.9 293.78L212.43 294.19L217.4 293.31L218.67 291.3L218.87 292.51L220.69 292.24L223.24 294.52Z"
						/>
					</mask>
					<path
						d="M223.24 294.52L221.63 310.51L222.03 315.01L231.91 325.09L234.06 328.72L234.66 336.71L232.51 344.1L233.72 354.99L230.63 359.29L238.83 367.35L240.44 371.65L242.19 373.4L241.78 379.58L245.95 385.62L248.5 395.03L253.21 403.49L253.07 406.85L256.03 411.96L255.09 414.38L256.97 415.18V416.93L254.15 418.61L256.03 423.65L261.8 422.84L266.57 426.13L270.34 423.65H272.29L274.3 431.17L272.42 441.12L279.27 450.39L278.33 458.72L279.41 459.52L276.58 471.21L278.47 476.19L277.53 479.54L278.53 483.71L276.65 487.81L278.6 489.49L282.5 499.57L282.63 509.51L277.39 517.97L269.73 526.57L261.13 525.23L251.59 531.81L233.05 540.95L217.33 543.77L196.37 537.05L188.17 528.99L180.65 530.87L169.23 529.39L161.57 527.11L156.33 541.35L149.61 545.65L141.01 542.29L133.35 534.63L124.35 533.69L116.69 548.47L113.87 557.61L107.15 560.97L100.97 549.01L86.59 564.73L67.11 549.95L57.97 554.25L50.72 534.63L48.97 533.83L52.87 526.84L52.13 523.21L55.75 517.57L55.69 504.54L54.21 503.73L54.34 501.58L52.93 500.1L56.36 495.27L57.84 486.73L60.39 484.92L64.02 478.6L71.47 469.13L70.6 466.51L67.98 459.86L62.61 452.6L59.18 441.92L56.56 441.59L55.02 439.91L54.28 427.75L65.29 422.17L66.17 418.07L63.01 411.62L57.37 408.73L59.72 406.99L85.79 409.2L84.11 401.55L78.13 397.11L83.23 384.62L91.43 371.11L93.11 371.78L92.03 374.94L94.12 377.16L94.05 381.12L102.04 378.1L100.5 375.61L104.66 367.82L103.25 363.86L105 361.03L105.81 362.85L112.39 366.07L118.17 363.39L120.38 365.33L123.34 365.06L129.66 371.72L134.29 370.31L137.78 371.92L143.76 368.89L153.1 374.87L154.92 375.21L155.86 373.73L154.58 373.13L154.71 369.83L153.51 368.63L154.18 364.26L152.23 363.05L153.57 362.85L151.89 361.24L152.9 360.16L152.03 359.02L152.7 358.21L151.62 357.88L163.38 342.36L167.14 331.2L167.21 326.3L154.18 306.01L152.43 287.27L154.78 286.19L167.01 286.39L170.57 284.78L170.44 285.99L172.05 286.39L177.96 285.79L186.76 287.87L188.44 286.8L190.05 287.47L190.99 291.16L193.14 291.9L194.49 290.69L196.91 290.49L199.19 293.92L202.82 291.5L204.9 293.78L212.43 294.19L217.4 293.31L218.67 291.3L218.87 292.51L220.69 292.24L223.24 294.52Z"
						stroke="black"
						class="fill-maroon-flush-300 hover:fill-maroon-flush-500"
						stroke-width="2"
						mask="url(#path-8-inside-8_78_1665)"
					/>
				</svg>
				<div class="grid grid-cols-2 gap-4">
					{#each impactStats as { title, value, description }}
						<div class="content-center rounded-3xl bg-white p-6">
							<p class="font-bitter text-maroon-flush-500 mb-4 text-3xl font-bold">{value}</p>
							<p class="font-bitter text-lg font-semibold">{title}</p>
							<small>{description}</small>
						</div>
					{/each}
				</div>
			</div>
		</div>
	</div>
</section>

<!-- from awareness to action -->
<section class="scroll-m-10 p-6 py-16">
	<div class="container mx-auto">
		<h3
			class="font-bitter after:bg-maroon-flush-600 mb-4 text-4xl font-medium after:ml-3 after:inline-block after:h-1 after:w-20 after:-translate-y-1/2 after:content-['']"
		>
			<span class="text-maroon-flush-600"> From Awareness </span> to Action
		</h3>
		<p>
			Every club is a space where girls speak up, support each other, and take real action to
			protect their peers.
		</p>
		<div class="mt-6 grid grid-cols-1 gap-4 md:grid-cols-2 lg:grid-cols-3">
			{#each activities as { icon, title, description }}
				<div class="bg-maroon-flush-50 rounded-2xl p-4">
					<div class="mb-3 flex h-11 w-11 items-center justify-center rounded-md bg-white">
						<img src={icon} alt="" class="h-6 w-6" />
					</div>
					<p class="mb-2 text-xl font-semibold">{title}</p>
					<p class="text-sm text-zinc-500">{description}</p>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- real girls real chaneg -->
<section class="scroll-m-10 p-6 py-16" id="stories">
	<div class="container mx-auto">
		<h3
			class="font-bitter after:bg-maroon-flush-600 mb-4 text-4xl font-medium after:ml-3 after:inline-block after:h-1 after:w-20 after:-translate-y-1/2 after:content-['']"
		>
			<span class="text-maroon-flush-600"> Real Girls. </span> Real Change
		</h3>
		<p>
			From escaping early marriage to returning to school — these are the voices of courage and
			community.
		</p>
		<div class="mt-10 grid grid-cols-1 gap-4 md:grid-cols-2 lg:grid-cols-3">
			{#each videoURLS as src}
				<iframe
					{src}
					title="YouTube video player"
					frameborder="0"
					allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
					referrerpolicy="strict-origin-when-cross-origin"
					allowfullscreen
					class="aspect-video h-56 w-full rounded-2xl"
					loading="lazy"
				></iframe>
			{/each}
		</div>
	</div>
</section>

<section class="scroll-m-10 p-6 py-16" id="contact">
	<div
		class="to-maroon-flush-300 container mx-auto rounded-3xl bg-gradient-to-r from-transparent p-6"
	>
		<div class="flex flex-wrap items-center lg:flex-nowrap">
			<img src="image/breaking barriers-cuate.svg" alt="" class="w-full max-w-sm" />
			<div class="group">
				<h3 class="font-bitter text-maroon-flush-800 mb-2 text-3xl font-semibold">
					When Girls Break Walls, Change Follows
				</h3>
				<p>
					Start a club, speak up, or take action — Balika Manch is where girls break through limits
					and lead their own future.
				</p>
				<div class="mt-4 flex gap-2">
					<button
						class="bg-maroon-flush-500 inline-block rounded-full px-4 py-3 font-medium text-white"
						>Call Phone</button
					>
					<button
						class="bg-maroon-flush-500 inline-block rounded-full px-4 py-3 font-medium text-white"
						>Send an Email</button
					>
				</div>
			</div>
		</div>
	</div>
</section>
