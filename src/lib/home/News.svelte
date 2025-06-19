<script>
	const news = [
		{
			image:
				'https://cdn.prod.website-files.com/67b6a9477efb8337b00f0de1/68484caf9adad2f6c64fff12_AIScheduleEngine_Hero_01.jpg',
			alt: 'IMAGE',
			title: 'Fastbreak AI Launches New AI Schedule Engine For Youth & Amateur Sports',
			date: 'DEC 31, 2025',
			description:
				'Fastbreak brings its pro-level AI Schedule Engine to youth sports, saving time and improving tournament operations.',
			Button: 'READ MORE'
		},
		{
			image:
				'https://cdn.prod.website-files.com/67b6a9477efb8337b00f0de1/6827947288c947912e696da5__FB_WP_Thumb2.png',
			alt: 'IMAGE',
			title: 'The NFL’s Schedule Was Built by AI. Fastbreak is the Company Leading the Way.',
			date: 'DEC 31, 2025',
			description:
				'The Washington Post explores how the NFL used artificial intelligence to create their 2025-2026 leauge schedule, and highlights Fastbreak AI.',
			Button: 'READ MORE'
		},
		{
			image:
				'https://cdn.prod.website-files.com/67b6a9477efb8337b00f0de1/68278bbadca20fc6bc8f49d9__Forbes_thumb.png',
			alt: 'IMAGE',
			title: 'How AI Is Changing Sports Scheduling. from Pro Leagues like TGL to Youth Tournaments',
			date: 'DEC 31, 2025',
			description:
				'From building smarter schedules for leagues like TGL to transforming operations in youth sports, Forbes calls Fastbreak AI “a scheduling power play.”',
			Button: 'READ MORE'
		}
	];

	const sports = [
		{
			image:
				'https://cdn.prod.website-files.com/67b6a9477efb8337b00f0de1/68472ab4321786efe842ecfc_RyanSilver_hero.jpg',
			alt: 'IMAGE',
			title: '1,000 Teams. 15 Venues. Zero Chaos.',
			date: 'DEC 31, 2025',
			description:
				'How Ryan Silver, CEO of Attitude for Gratitude, uses Fastbreaks AI Schedule Engine to run 1,000-team tournaments.',
			Button: 'READ MORE'
		},
		{
			image:
				'https://cdn.prod.website-files.com/67b6a9477efb8337b00f0de1/68372a3003152c9d0f1cc27f_BLOG_HERO_Spikeball.webp',
			alt: 'IMAGE',
			title: 'Why Experiential Marketing Isn’t Optional For Consumer Brands in the Gen Z Era',
			date: 'DEC 31, 2025',
			description:
				'Gen Z doesnt just influence purchases, they drive them. If youre not engaging families, youre missing a chance to build longterm loyalty.',
			Button: 'READ MORE'
		},
		{
			image:
				'https://cdn.prod.website-files.com/67b6a9477efb8337b00f0de1/682df19a8f7f0125b9b8c063_BLOG_HERO_Parents.webp',
			alt: 'IMAGE',
			title: 'Why Experiential Marketing Isn’t Optional For Consumer Brands in the Gen Z Era',
			date: 'DEC 31, 2025',
			description:
				'What Parents Really Want from Hotel Booking Policies at Stay-to-Play Tournaments',
			Button: 'READ MORE'
		}
	];
</script>

<div class="mx-auto flex w-full max-w-screen-2xl flex-col gap-6 px-6 text-black">
	<div class="border-neutral rounded-lg border">
		<div class=" bg-white">
			<div class="flex justify-between p-6">
				<h5>Newsroom</h5>
				<div>
					<button
						class="btn btn-base-content group flex items-center justify-start gap-2 text-center"
					>
						NEWS & PRESS
						<span
							class="transform text-2xl transition-all duration-300 ease-in-out group-hover:translate-x-2"
						>
							&rarr;
						</span>
					</button>
				</div>
			</div>
			<hr class=" border-base-content w-full border" />

			<div class="flex flex-col gap-12 p-6">
				<div>
					<h5 class="text-6xl font-black tracking-tighter">NEWS & <br /> INSIGHTS</h5>
					<p class="mt-4 max-w-xl text-gray-500">
						Lorem, ipsum dolor sit amet consectetur adipisicing elit. Enim nam natus, repellendus
						nisi facere aspernatur, assumenda, nesciunt aperiam ratione animi ipsa totam minus?
						Repellat saepe temporibus labore perspiciatis velit beatae.
					</p>
				</div>

				<div>
					<div class="flex justify-between">
						<p class="text-lg font-semibold">Latest News & Press</p>
						<p class="text-gray-500">ALL NEWS & PRESS</p>
					</div>
					<div class="my-4 grid md:grid-cols-2 lg:grid-cols-3 gap-4">
						{#each news as { image, alt, title, date, description, Button }}
							<a href="/" class="flex flex-col rounded-xl bg-gray-100">
								<img src={image} {alt} class="h-80 rounded-t-xl" />
								<div class="flex flex-grow flex-col gap-2 p-2">
									<p class="text-lg font-bold tracking-tight">{title}</p>
									<p class="text-base-content font-semibold">{date}</p>
									<p class="text-neutral flex-grow font-semibold">{description}</p>
									<button class="btn btn-neutral mt-auto h-12 w-full">{Button}</button>
								</div>
							</a>
						{/each}
					</div>
					<div class="flex justify-between">
						<p class="text-lg font-semibold">Latest Insights From Our Blog</p>
						<p class="text-gray-500">ALL INSIGHTS</p>
					</div>
					<div class="mt-4 grid md:grid-cols-2 lg:grid-cols-3 gap-4">
						{#each sports as { image, alt, title, date, description, Button }}
							<a href="/" class="flex flex-col rounded-xl bg-gray-100">
								<img src={image} {alt} class="h-80 rounded-t-xl" />
								<div class="flex flex-grow flex-col gap-2 p-2">
									<p class="text-lg font-bold tracking-tight">{title}</p>
									<p class="text-base-content font-semibold">{date}</p>
									<p class="text-neutral flex-grow font-semibold">{description}</p>
									<button class="btn btn-neutral mt-auto h-12 w-full">{Button}</button>
								</div>
							</a>
						{/each}
					</div>
				</div>
			</div>
		</div>
		<div class="m-10 grid sm:grid-cols-2 gap-4 text-white">
			<div class="bg-neutral rounded-lg p-4">
				<div class="flex flex-col items-start gap-4">
					<img
						src="https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67d898b493ca2655c7897f45_5336565ec280e25933fe75e0e443a8f8_Fastbreak_Impact_wtype_rgb.svg"
						alt="impact"
						class="h-12"
					/>
					<p class="lg:text-lg tracking-wide">
						Lorem ipsum dolor sit, amet consectetur adipisicing elit. Adipisci odit qui sapiente.
						Blanditiis officiis amet maiores corrupti aliquid nihil ea voluptas vero! Asperiores
						natus ad veniam, ducimus omnis reprehenderit vero?
					</p>
					<div>
						<button
							class="btn btn-base-content group flex items-center justify-start gap-2 text-center"
						>
							LEARN MORE
							<span
								class="transform text-2xl transition-all duration-300 ease-in-out group-hover:translate-x-2"
							>
								&rarr;
							</span>
						</button>
					</div>
				</div>
				<div>
					<img
						src="https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67ee72301ea8c01347d4bc02_kids-soccer.webp"
						alt="playing soccer"
					/>
				</div>
			</div>

			<div class="bg-neutral flex h-full flex-col justify-between rounded-lg p-4">
				<div>
					<h6 class="sm:text-2xl font-bold tracking-tighter">QUESTION?</h6>
					<div class="flex justify-end">
						<img
							src="https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67b6a9477efb8337b00f0e6c_EARTH%20GLOBE%20GRAPHIC%20(5).avif"
							alt="system"
							class="h-96 opacity-20"
						/>
					</div>
				</div>

				<div>
					<button
						class="btn btn-base-content group mb-6 flex items-center justify-start gap-2 text-center"
					>
						Contact Us
						<span
							class="transform text-2xl transition-all duration-300 ease-in-out group-hover:translate-x-2"
						>
							&rarr;
						</span>
					</button>
					<p class="sm:text-xl">
						We're here to help!
						<strong class="text-secondary font-bold underline">Contact Us</strong>
					</p>
				</div>
			</div>
		</div>
	</div>
</div>
