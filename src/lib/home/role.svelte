<script>
	import Football from '$lib/image/American Football Silhouette Clipart - Free Png, Svg, Vector Images _ Neoclipart.jpg';
	import Addidas from '$lib/image/Descargar logotipo de adidas símbolo negro icono de diseño de ropa ilustración de vector de fútbol abstracto con fondo blanco.jpg';
	import Tennis from '$lib/image/Free printable Handball stencils and templates.jpg';
	import Footballs from '$lib/image/Football Logo Black And White.jpg';
	import Volleyball from '$lib/image/Free printable Volleyball stencils and templates.jpg';
	import UnderArmor from '$lib/image/Logo- The Under Armor logo_.jpg';
	import Nba from '$lib/image/NBA.jpg';
	import Mamba from '$lib/image/Kobe Logo - Black Mamba - PNG Logo Vector Brand Downloads (SVG, EPS).jpg';

	const role = [
		{
			title: 'FASTBREAK PRO',
			image:
				'https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67ee7230acd2ce90bf4ee7c1_basketball-1.webp',
			alt: 'FASTBREAK PRO image',
			selection: 'PRO SPORTS',
			description:
				'Advanced AI schedule creation and optimization improves efficiency, ensures fairness, and maximizes broadcast & ticket revenue.',
			button: 'SEE PRO IN ACTION'
		},
		{
			title: 'FASTBREAK CONNECT',
			image:
				'https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67ee7230a9d2088626590e44_drinks.webp',
			alt: 'FASTBREAK CONNECT image',
			selection: 'BRAND & AGENCIES',
			description:
				'Connect with youth athletes and their families through scalable on-site activations, branded experiences, and tournaments.',
			button: 'DISCOVER CONNECT'
		},
		{
			title: 'FASTBREAK COMPETE',
			image:
				'https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67ee7230387e58264aabb72c_volleyball.webp',
			alt: 'FASTBREAK COMPETE image',
			selection: 'AMATEUR & YOUTH SPORTS EVENTS',
			description:
				'Powerful registration, scheduling, and event management for youth, high school, and amateur sports events, leagues & tournaments.',
			button: 'EXPLORE COMPETE'
		}
	];

	const firstLogo = [
		{ image: Football, alt: 'Football' },
		{ image: Addidas, alt: 'Addidas' },
		{ image: Tennis, alt: 'Tennis' },
		{ image: Footballs, alt: 'Footballs' }
	];

	const secondLogo = [
		{ image: Volleyball, alt: 'Volleyball' },
		{ image: UnderArmor, alt: 'Under Armor' },
		{ image: Nba, alt: 'NBA' },
		{ image: Mamba, alt: 'Steph Curry' }
	];

	const operation = [
		{
			image:
				'https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67ee5b2ab2735be2195ff592_calendar-range-thin.svg',
			src: 'book',
			title: 'Smarter Scheduling',
			description: 'AI-driven optimization for fairness and efficiency.'
		},
		{
			image:
				'https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67ee5b2a65ab61f6a30f2133_plane-arrival-thin.svg',
			src: 'airplain',
			title: 'Less Travel, More Play',
			description: 'Reduce unnecessary travel to reduce costs & fatigue.'
		},
		{
			image:
				'https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67ee5b2aff0ec372cf1ab112_chart-mixed-up-circle-dollar-thin.svg',
			src: 'price',
			title: 'Maximize Revenue',
			description: 'Integrate sponsors to fund more events & programs.'
		},
		{
			image:
				'https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67ee5b2a796001c881ce9322_arrow-progress-thin.svg',
			src: 'operation',
			title: 'Seamless Operations',
			description: 'Streamline logistics and simplify management.'
		}
	];
</script>

<div class="mx-auto flex w-full max-w-screen-2xl flex-col gap-6 px-6">
	<div class="flex flex-col gap-6">
		<div class="border-secondary flex flex-col rounded-2xl border text-white">
			<div class="flex flex-col gap-10 px-6 py-10">
				<div>
					<h2 class="mb-4 text-4xl font-bold tracking-wider ">
						AI-DRIVEN <strong class="text-primary">SOLUTIONS</strong> <br /> TO POWER YOUR GAME
					</h2>
					<p class="text-sm max-md:text-xs">
						From professional leagues to youth tournaments, Fastbreak's b cutting-edge <br /> AI helps
						you optimize scheduling, enhance engagement, and maximize impact.
					</p>
				</div>
			</div>
			<div class="flex flex-col gap-4 px-6 py-2">
				<div>
					<h3 class=" font-bold md:text-xl">
						<strong class="text-primary">01</strong> <span> Choose Your Role</span>
					</h3>
				</div>
				<div class="grid sm:grid-cols-3 gap-3 md:gap-6">
					{#each role as { title, image, alt, selection, description, button }}
						<div
							class="border-secondary hover:shadow-secondary flex flex-col gap-5 rounded-2xl border p-2 md:p-4 hover:border-2 hover:shadow-lg"
						>
							<div class="flex flex-1 max-md:text-center flex-col gap-5">
								<h4 class="text-sm font-bold ">{title}</h4>
								<img src={image} {alt} class="h-auto w-full" />
								<p class="text-primary text-lg font-semibold max-lg:text-xs">{selection}</p>
								<p class="text-sm max-lg:text-xs 2xl:mr-30">{description}</p>
							</div>
							<div class="flex justify-center xl:mt-10 xl:justify-end">
								<button
									class="btn max-lg:btn-xs btn-primary group h-12 gap-2 text-center max-lg:h-10"
								>
									{button}
									<span
										class="transform transition-all duration-300 ease-in-out group-hover:translate-x-2 lg:text-2xl"
									>
										&rarr;
									</span>
								</button>
							</div>
						</div>
					{/each}
				</div>
			</div>

			<div class="grid sm:grid-cols-2 bg-white lg:px-4 text-black">
				<div class="flex items-end py-14">
					<div class="flex flex-col gap-10">
						<h2 class="mx-2 max-md:text-4xl max-lg:text-5xl text-6xl font-black tracking-tighter">
							Powering Schedules for the World’s Premier Leagues
						</h2>
						<p class="mx-4 text-lg font-semibold text-gray-500">
							Elevate your league with Fastbreak’s proven expertise, trusted by global sports
							leaders to optimize schedules and enhance performance seamlessly.
						</p>
					</div>
				</div>

				<div class="grid max-sm:h-96 sm:h-[600px] sm:grid-cols-2 items-center justify-center gap-2 overflow-hidden">
					<div class="animate-scroll-up mx-auto flex flex-col gap-2">
						{#each [...firstLogo, ...firstLogo] as { image, alt }}
							<div class="rounded-lg border-2">
								<img src={image} {alt} class="sm:mx-4 h-55 xl:h-60  sm:w-30 md:w-34 lg:w-50 xl:w-80 object-contain" />
							</div>
						{/each}
					</div>

					<div class="animate-scroll-down mx-auto flex flex-col gap-2">
						{#each [...secondLogo, ...secondLogo] as { image, alt }}
							<div class="rounded-lg border-2">
								<img src={image} {alt} class="sm:mx-4 h-55 xl:h-60  sm:w-30 md:w-34 lg:w-50 xl:w-80 object-contain" />
							</div>
						{/each}
					</div>
				</div>
			</div>
		</div>

		<div class="border-secondary flex flex-col rounded-2xl border text-white">
			<div class="flex justify-between p-5">
				<h3 class="text-lg font-semibold">
					<strong class="text-primary">02</strong> Why Fastbreak
				</h3>
				<button class="btn btn-secondary">Learn More</button>
			</div>
			<hr class=" border-secondary w-full border" />

			<div class="p-6">
				<div class="grid lg:grid-cols-2 xl:grid-cols-3">
					<div class="pt-10">
						<h2 class="mb-6 sm:text-2xl md:text-4xl lg:text-6xl font-black tracking-tighter">
							<strong class="text-primary">Optimizing</strong> Sports Operations
						</h2>
						<p class="md:max-w-xl xl:text-lg">
							Fastbreak AI products optimize every part of sports. From scheduling and event
							management to travel, ticketing, and brand activations, each product is purpose-built
							to simplify operations, unlock new revenue, and help organizations run faster,
							smarter, and more efficiently.
						</p>
					</div>
					<div class="xl:col-span-2 grid">
						<img
							src="https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67eda30677768ebffc36f3da_b57eee2dc4eee777dc4a07285bb79f6d_optimization.webp"
							alt="optimization"
							class="w-full"
						/>
					</div>
				</div>

				<div class="grid lg:grid-cols-2 mt-10">
					<div class="grid grid-cols-2 gap-10">
						{#each operation as { image, src, title, description }}
							<div class="flex flex-col gap-2">
								<img src={image} alt={src} class="max-sm:size-10 sm:size-16 brightness-0 invert filter" />
								<h5 class="mb-1 sm:text-xl font-bold">{title}</h5>
								<p class="font-semibold max-sm:text-xs text-gray-500">{description}</p>
							</div>
						{/each}
					</div>
				</div>
			</div>
		</div>
	</div>
</div>
<div class="relative h-full w-screen overflow-hidden bg-cover bg-center bg-no-repeat">
	<div
		class="absolute inset-0 bg-[url('https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67cf9046ac6c6d99e011660b_wave-2.webp')] bg-cover bg-center bg-no-repeat opacity-10"
	></div>

	<div class="relative z-10 grid place-items-center p-10 text-center text-white">
		<img
			src="https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67b6a9477efb8337b00f0f58_erervfd.avif"
			alt="avif"
			class="size-10"
		/>
		<h5 class="my-4 max-w-3xl sm:text-2xl font-black">
			Fastbreak has been a valued partner with the Big East for a number of years. With the most
			difficult and complex scheduling challenges in college sports, the Big East basketball slate
			has been expertly developed, fine-tuned and refined with the power of Fastbreak AI - an
			industry leader.
		</h5>
		<h6 class="text-lg font-bold">Mike Coyne</h6>
		<p class="mb-4 text-lg font-bold">Associate Commissioner, Big East</p>
		<img
			src="https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67d8b2ee3feb31d090b4c86f_Big_East_Conference_logo-1024x210.png"
			alt="conference logo"
			class="mt-4 w-30"
		/>
	</div>
</div>

<style>
	@keyframes scrollUp {
		0% {
			transform: translateY(0);
		}
		100% {
			transform: translateY(-50%);
		}
	}

	@keyframes scrollDown {
		0% {
			transform: translateY(-50%);
		}
		100% {
			transform: translateY(0);
		}
	}

	.animate-scroll-up {
		animation: scrollUp 20s linear infinite;
	}

	.animate-scroll-down {
		animation: scrollDown 20s linear infinite;
	}
</style>
