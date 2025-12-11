<script lang="ts">
	// Community badges
	const badges = [
		{ name: 'Godot', width: 80 },
		{ name: 'itch.io', width: 90 },
		{ name: 'GameDev', width: 80 },
		{ name: 'IndieDB', width: 90 },
		{ name: 'Steam', width: 70 },
		{ name: 'Unity', width: 70 },
		{ name: 'Unreal', width: 80 },
		{ name: 'GameJolt', width: 85 },
		{ name: 'Newgrounds', width: 95 },
		{ name: 'Kongregate', width: 100 }
	];
</script>

<section class="relative pt-32 pb-16 px-6 md:px-12 max-w-7xl mx-auto min-h-screen flex flex-col justify-between">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
		<div class="z-10">
			<h1 class="text-6xl md:text-7xl lg:text-8xl font-display font-medium text-gray-900 leading-[0.9] tracking-tight mb-8">
				Build games,<br><span class="text-primary-600">faster</span>
			</h1>
			
			<div class="relative w-12 h-12 mb-8">
				<!-- Goji mascot wink animation -->
				<svg viewBox="0 0 24 24" fill="none" class="w-8 h-8 text-primary-500 absolute top-0 left-0 animate-bounce">
					<circle cx="12" cy="12" r="10" fill="currentColor" opacity="0.8"/>
					<path d="M8 10h.01M16 10h.01M8 14s1.5 2 4 2 4-2 4-2" stroke="white" stroke-width="2" stroke-linecap="round"/>
				</svg>
			</div>

			<div class="space-y-6 max-w-lg">
				<p class="font-mono text-sm text-gray-700 uppercase tracking-wider leading-relaxed">
					Generate Godot scripts and scenes<br>
					through natural language.<br>
					Ship your game idea, today.
				</p>

				<div class="flex flex-col items-start gap-3">
					<button class="bg-primary-600 text-white px-6 py-3 rounded text-sm font-medium hover:bg-primary-700 transition-colors flex items-center gap-2">
						Download for Free
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
					</button>
					<p class="text-[10px] text-gray-500 font-mono uppercase tracking-wide">
						100 free credits • macOS & Windows
					</p>
				</div>
			</div>
		</div>

		<div class="relative h-[400px] lg:h-[600px] w-full flex items-center justify-center">
			<!-- Game development illustration -->
			<div class="absolute inset-0 flex items-center justify-center">
				<img src="/generated/image-solo-indie-game-developer-working-at-des-1765491622951-0.webp" alt="Indie game developer working with Godot" class="w-full h-full object-cover rounded-lg shadow-2xl" />
			</div>
		</div>
	</div>

	<div class="mt-20 border-t border-gray-300 pt-8">
		<div class="flex items-center gap-2 text-[10px] font-mono uppercase tracking-wider text-gray-600 mb-6">
			Trusted by indie developers worldwide
			<a href="/" class="text-primary-600 hover:underline flex items-center gap-1">
				Join the community <span class="text-xs">♥</span> ->
			</a>
		</div>
		
		<div class="grid grid-cols-2 md:grid-cols-5 gap-8 opacity-60 grayscale">
			{#each badges as badge}
				<div class="h-8 flex items-center justify-center border border-gray-300/50 rounded bg-gray-100/50">
					<span class="text-xs font-bold text-gray-500">{badge.name}</span>
				</div>
			{/each}
		</div>
	</div>
</section>
