<section class="bg-gradient-to-br from-accent-yellow/10 via-accent-pink/10 to-accent-orange/10 py-24 px-6 md:px-12 relative overflow-hidden">
	<!-- Playful decorative elements -->
	<div class="absolute top-20 left-10 w-24 h-24 border-4 border-accent-pink/30 rounded-full animate-pulse"></div>
	<div class="absolute bottom-20 right-20 w-32 h-32 border-4 border-accent-yellow/30 rotate-45 animate-pulse" style="animation-delay: 1s;"></div>
	
	<div class="max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-2 gap-12 items-center relative z-10">
		<div>
			<span class="text-sm text-accent-orange font-bold mb-4 block flex items-center gap-2">
				<span class="animate-bounce">🧠</span> Super smart AI
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-6 leading-[0.95]">
				Knows your game<br>inside out 🔍
			</h2>
			<p class="text-base text-gray-700 max-w-md mb-8 leading-relaxed">
				Goji reads your whole project like a book! It learns your style and makes code that fits right in. No awkward copy-paste vibes here.
			</p>
			
			<button class="bg-gradient-to-r from-accent-orange to-primary-600 text-white px-6 py-3 rounded-full text-sm font-bold hover:scale-105 transition-transform flex items-center gap-2 shadow-lg w-fit">
				See how it works ✨ →
			</button>
		</div>

		<div class="relative h-[400px] w-full flex items-center justify-center">
			<!-- Graph Visualization Placeholder -->
			<div class="absolute inset-0">
				<!-- In a real implementation, this would be a canvas or complex SVG -->
				<svg width="100%" height="100%" viewBox="0 0 400 300" class="overflow-visible">
					<!-- Nodes -->
                    <g fill="#D97706" stroke="#fff" stroke-width="1">
                        <circle cx="200" cy="150" r="6" />
                        <circle cx="150" cy="100" r="4" />
                        <circle cx="250" cy="100" r="4" />
                        <circle cx="150" cy="200" r="4" />
                        <circle cx="250" cy="200" r="4" />
                        <circle cx="100" cy="150" r="3" />
                        <circle cx="300" cy="150" r="3" />
                        
                        <!-- Random scattered nodes -->
                        <circle cx="180" cy="80" r="3" />
                        <circle cx="220" cy="80" r="3" />
                        <circle cx="180" cy="220" r="3" />
                        <circle cx="220" cy="220" r="3" />
                    </g>
                    
                    <!-- Edges -->
                    <g stroke="#D97706" stroke-width="0.5" opacity="0.6">
                        <line x1="200" y1="150" x2="150" y2="100" />
                        <line x1="200" y1="150" x2="250" y2="100" />
                        <line x1="200" y1="150" x2="150" y2="200" />
                        <line x1="200" y1="150" x2="250" y2="200" />
                        <line x1="150" y1="100" x2="100" y2="150" />
                        <line x1="250" y1="100" x2="300" y2="150" />
                        <line x1="150" y1="200" x2="100" y2="150" />
                        <line x1="250" y1="200" x2="300" y2="150" />
                        
                        <!-- More edges -->
                         <line x1="150" y1="100" x2="180" y2="80" />
                         <line x1="250" y1="100" x2="220" y2="80" />
                    </g>
				</svg>
                <div class="absolute inset-0 flex items-center justify-center pointer-events-none">
                     <img src="https://placehold.co/600x400/transparent/D97706?text=Game+Project+Graph" alt="Graph" class="opacity-50" />
                </div>
			</div>
		</div>
	</div>
    
    <!-- Background Grid Pattern -->
    <div class="absolute inset-0 z-0 opacity-10" 
        style="background-image: linear-gradient(#000 1px, transparent 1px), linear-gradient(90deg, #000 1px, transparent 1px); background-size: 40px 40px;">
    </div>
</section>
