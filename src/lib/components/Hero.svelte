<script lang="ts">
	// Community badges with fun colors
	const badges = [
		{ name: 'Godot', color: 'bg-blue-500' },
		{ name: 'itch.io', color: 'bg-red-500' },
		{ name: 'GameDev', color: 'bg-purple-500' },
		{ name: 'IndieDB', color: 'bg-orange-500' },
		{ name: 'Steam', color: 'bg-blue-600' },
		{ name: 'Unity', color: 'bg-gray-800' },
		{ name: 'Unreal', color: 'bg-gray-900' },
		{ name: 'GameJolt', color: 'bg-green-500' },
		{ name: 'Newgrounds', color: 'bg-yellow-500' },
		{ name: 'Kongregate', color: 'bg-red-600' }
	];
</script>

<section class="relative pt-32 pb-16 px-6 md:px-12 max-w-7xl mx-auto min-h-screen flex flex-col justify-between overflow-hidden">
	<!-- Playful floating shapes in background -->
	<div class="absolute top-20 left-10 w-32 h-32 bg-accent-pink/20 rounded-full blur-3xl animate-pulse"></div>
	<div class="absolute top-40 right-20 w-40 h-40 bg-accent-yellow/20 rounded-full blur-3xl animate-pulse" style="animation-delay: 1s;"></div>
	<div class="absolute bottom-40 left-1/4 w-36 h-36 bg-accent-orange/20 rounded-full blur-3xl animate-pulse" style="animation-delay: 2s;"></div>
	
	<!-- Fun geometric shapes -->
	<div class="absolute top-1/4 right-10 w-12 h-12 border-4 border-accent-pink rotate-12 animate-bounce" style="animation-delay: 0.5s;"></div>
	<div class="absolute bottom-1/3 left-20 w-16 h-16 bg-accent-yellow/30 rounded-lg rotate-45 animate-bounce" style="animation-delay: 1.5s;"></div>
	
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center relative z-10">
		<div>
			<h1 class="text-6xl md:text-7xl lg:text-8xl font-display font-medium text-gray-900 leading-[0.9] tracking-tight mb-8">
				Build games,<br><span class="bg-gradient-to-r from-accent-orange via-accent-pink to-primary-600 bg-clip-text text-transparent">faster</span> ⚡
			</h1>
			
			<div class="relative w-20 h-20 mb-8">
				<!-- Enhanced Goji mascot with playful animation -->
				<svg viewBox="0 0 24 24" fill="none" class="w-16 h-16 text-accent-orange absolute top-0 left-0 animate-bounce">
					<circle cx="12" cy="12" r="10" fill="currentColor" opacity="0.9"/>
					<circle cx="9" cy="10" r="1.5" fill="white"/>
					<circle cx="15" cy="10" r="1.5" fill="white"/>
					<path d="M8 14s1.5 2 4 2 4-2 4-2" stroke="white" stroke-width="2" stroke-linecap="round"/>
					<!-- Winking eye overlay -->
					<path d="M14 10h2" stroke="white" stroke-width="1.5" stroke-linecap="round" class="animate-pulse"/>
				</svg>
				<!-- Sparkles around Goji -->
				<div class="absolute -top-1 -right-1 text-accent-yellow text-xl animate-ping">✨</div>
				<div class="absolute -bottom-1 -left-1 text-accent-pink text-sm animate-ping" style="animation-delay: 0.5s;">✨</div>
			</div>

			<div class="space-y-6 max-w-lg">
				<p class="text-lg text-gray-700 leading-relaxed">
					Turn your game ideas into real Godot code with just plain English. No coding wizardry required! 🎮
				</p>

				<div class="flex flex-col items-start gap-3">
					<button class="bg-gradient-to-r from-accent-orange to-primary-600 text-white px-8 py-4 rounded-full text-base font-bold hover:scale-105 transition-transform flex items-center gap-2 shadow-lg hover:shadow-xl">
						Get Goji free! 🚀
						<svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
					</button>
					<p class="text-xs text-gray-600">
						100 free credits to start • Works on Mac & Windows 💻
					</p>
				</div>
			</div>
		</div>

		<div class="relative h-[400px] lg:h-[600px] w-full flex items-center justify-center">
			<!-- Game development illustration with playful border -->
			<div class="absolute inset-0 flex items-center justify-center">
				<div class="relative w-full h-full">
					<!-- Fun colorful border effect -->
					<div class="absolute -inset-2 bg-gradient-to-r from-accent-pink via-accent-yellow to-accent-orange rounded-2xl blur-lg opacity-30 animate-pulse"></div>
					<img src="/generated/image-solo-indie-game-developer-working-at-des-1765491622951-0.webp" alt="Indie game developer working with Godot" class="relative w-full h-full object-cover rounded-2xl" />
				</div>
			</div>
		</div>
	</div>

	<div class="mt-20 border-t-2 border-dashed border-gray-300 pt-8 relative z-10">
		<div class="flex items-center gap-2 text-sm text-gray-700 mb-6">
			<span class="animate-pulse">💜</span>
			Loved by indie devs everywhere
			<a href="/" class="text-accent-orange hover:text-accent-pink transition-colors font-bold flex items-center gap-1 hover:gap-2 transition-all">
				Join the fun →
			</a>
		</div>
		
		<div class="grid grid-cols-2 md:grid-cols-5 gap-4">
			{#each badges as badge}
				<div class="h-12 flex items-center justify-center border-2 border-gray-200 rounded-xl {badge.color} text-white font-bold text-sm hover:scale-110 transition-transform cursor-pointer shadow-md hover:shadow-lg">
					{badge.name}
				</div>
			{/each}
		</div>
	</div>
</section>
