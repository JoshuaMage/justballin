<script>
	import '../app.css';
	import Footer from '$lib/footer.svelte';
	let { children } = $props();

	let showMobileMenu = $state(false);
</script>

<nav class="max-lg:mx-4 max-lg:my-8 lg:m-8 font-bold">
	<div class="grid grid-cols-3 items-center md:grid-cols-4">
		<a href="/" class="text-3xl">JustBallin</a>

		<div class="hidden items-center max-xl:gap-4 md:col-span-2 md:flex xl:justify-around">
			<a href="/amateur" class="text-primary font-serif text-xs hover:underline">AMATEUR</a>
			<a href="/pro" class="text-primary font-serif text-xs hover:underline">PRO</a>
			<a href="/brands" class="text-primary font-serif text-xs hover:underline">BRANDS</a>
			<a href="/product" class="font-serif text-xs hover:underline">PRODUCTS</a>
			<a href="/role" class="font-serif text-xs hover:underline">ROLE</a>
			<a href="/company" class="font-serif text-xs hover:underline">COMPANY</a>
		</div>

		<div class="hidden items-center justify-end gap-2 md:flex xl:gap-10">
			<button class="btn max-lg:btn-sm btn-primary">LOGIN</button>
			<a href="/contact" class="max-lg:text-sm">CONTACT</a>
		</div>

		<div class="col-span-2 flex justify-end md:hidden">
			<button onclick={() => (showMobileMenu = !showMobileMenu)} class="text-2xl"> ☰ </button>
		</div>
	</div>

	{#if showMobileMenu}
		<div class="mt-4 flex flex-col gap-2 text-sm md:hidden">
			<a href="/amateur" class="text-primary font-serif hover:underline">AMATEUR</a>
			<a href="/pro" class="text-primary font-serif hover:underline">PRO</a>
			<a href="/brands" class="text-primary font-serif hover:underline">BRANDS</a>
			<a href="/product" class="font-serif hover:underline">PRODUCTS</a>
			<a href="/role" class="font-serif hover:underline">ROLE</a>
			<a href="/company" class="font-serif hover:underline">COMPANY</a>
			<hr class="border-secondary my-2 max-md:hidden" />
			<button class="btn btn-sm btn-primary w-30">LOGIN</button>
			<a href="/contact">CONTACT</a>
		</div>
	{/if}
</nav>

<div class="border-secondary border-b-1"></div>

{@render children()}

<div class="mt-10">
	<Footer />
</div>
