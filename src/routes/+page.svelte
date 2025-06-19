<script>
	import Role from '$lib/home/role.svelte';
	import News from '$lib/home/News.svelte';
</script>

<div class="flex h-full w-full items-center justify-center">
	<div class="w-full">
		<div class="flex flex-col items-center gap-10 overflow-hidden font-[unset]">
			<div
				class="grid h-96 max-lg:place-items-center xl:h-screen w-screen xl:grid-cols-2 bg-cover bg-center bg-no-repeat"
				style="background-image: url('https://cdn.prod.website-files.com/67b6a9467efb8337b00f0d4c/67f397b23d1b36971603bf2d_ebd2b9ecda1908df34f12d3a2f1e8c1b_home-hero.jpg');"
			>
				<section class="max-xl:h-96 mx-auto flex flex-col max-xl:items-center justify-center gap-5 p-4 xl:p-14">
					<h2 class="max-sm:text-lg sm:text-2xl md:text-3xl lg:text-4xl xl:text-7xl  leading-tight font-black tracking-tighter text-white">
						The Ultimate <strong class="text-primary">AI-Powered</strong><br />
						Sports Operations Engine
					</h2>
					<p class="lg:text-lg font-semibold text-white">
						Intelligent software for sports league scheduling, tournament management, and
						experiential sponsorship for brands.
					</p>
					<div>
						<button class="btn btn-primary group flex items-center justify-start gap-2 text-center">
							Choose Your Role
							<span
								class="transform text-2xl transition-all duration-300 ease-in-out group-hover:translate-x-2"
							>
								&rarr;
							</span>
						</button>
					</div>
				</section>
				<section></section>
			</div>

			<Role />
			<News />
		</div>
	</div>
</div>
