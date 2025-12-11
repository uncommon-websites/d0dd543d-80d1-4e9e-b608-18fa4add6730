<script lang="ts">
	import { onMount } from 'svelte';
	
	let isScrolled = false;

	onMount(() => {
		const handleScroll = () => {
			isScrolled = window.scrollY > 20;
		};
		window.addEventListener('scroll', handleScroll);
		return () => window.removeEventListener('scroll', handleScroll);
	});
</script>

<header class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 px-6 py-4 flex items-center justify-between {isScrolled ? 'bg-[#EAEAE8]/90 backdrop-blur-md border-b border-gray-200' : 'bg-transparent'}">
	<div class="flex items-center gap-8">
		<a href="/" class="flex items-center gap-2 text-brand-dark font-medium text-xl tracking-tight">
			<div class="w-6 h-6 bg-primary-600 rounded-sm flex items-center justify-center text-white text-xs font-bold">G</div>
			Goji
		</a>
		
		<nav class="hidden md:flex items-center gap-6 text-sm font-medium text-gray-600">
			<a href="#pricing" class="hover:text-gray-900 transition-colors">Pricing</a>
			<button class="flex items-center gap-1 hover:text-gray-900 transition-colors group">
				Features 
				<svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="group-hover:rotate-180 transition-transform"><path d="m6 9 6 6 6-6"/></svg>
			</button>
			<a href="#docs" class="hover:text-gray-900 transition-colors">Docs</a>
			<button class="flex items-center gap-1 hover:text-gray-900 transition-colors group">
				Resources
				<svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="group-hover:rotate-180 transition-transform"><path d="m6 9 6 6 6-6"/></svg>
			</button>
			<a href="#blog" class="hover:text-gray-900 transition-colors">Blog</a>
		</nav>
	</div>

	<div class="flex items-center gap-4">
		<a href="#signin" class="text-sm font-medium text-white bg-black px-4 py-2 rounded hover:bg-gray-800 transition-colors">Sign In</a>
		<a href="#start" class="text-sm font-medium text-white bg-primary-600 px-4 py-2 rounded hover:bg-primary-700 transition-colors shadow-sm">Download</a>
	</div>
</header>
