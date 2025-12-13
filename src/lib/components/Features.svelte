<script lang="ts">
	import FeatureCard from './FeatureCard.svelte';
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto relative" id="features">
    <!-- Background Grid Pattern -->
    <div class="absolute inset-0 z-0 opacity-30 pointer-events-none" 
        style="background-image: linear-gradient(#ccc 1px, transparent 1px), linear-gradient(90deg, #ccc 1px, transparent 1px); background-size: 40px 40px; mask-image: linear-gradient(to bottom, transparent, black 10%, black 90%, transparent);">
    </div>

	<div class="flex flex-col md:flex-row justify-between items-start md:items-end mb-16 gap-6 relative z-10">
		<div>
			<span class="text-sm text-accent-orange font-bold mb-4 block flex items-center gap-2">
				<span class="animate-pulse">🤖</span> Your AI game buddy
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-4">
				From idea to playable game 🎮
			</h2>
			<p class="text-base text-gray-700 max-w-lg">
				Goji turns your wild game ideas into real Godot code. Just tell it what you want!
			</p>
		</div>
		
		<button class="bg-gradient-to-r from-gray-900 to-gray-700 text-white px-6 py-3 rounded-full text-sm font-bold hover:scale-105 transition-transform flex items-center gap-2 shadow-lg">
			Watch the magic ✨ →
		</button>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-2 gap-6">
		<FeatureCard 
			subtitle="[ NATURAL LANGUAGE ]"
			title="Generate scripts with<br>simple commands"
			description="Type what you want in plain English. Goji generates GDScript code that matches your game's architecture."
			tagColor="bg-primary-600"
			tagIcon="arrow"
            imageSrc="/generated/image-close-up-of-hands-typing-code-on-mechani-1765491626213-1.webp"
		/>
		
		<FeatureCard 
			subtitle="[ SCENE BUILDER ]"
			title="Create complete scenes<br>instantly"
			description="Describe your scene and Goji builds it with nodes, properties, and connections ready to go."
			tagColor="bg-accent-orange"
			tagIcon="plus"
            imageSrc="/generated/image-computer-screen-showing-a-2d-game-scene--1765491628476-2.webp"
		/>
		
		<FeatureCard 
			subtitle="[ MULTI-MODEL AI ]"
			title="Choose the best AI<br>for each task"
			description="Access Claude, Gemini, and more from one interface. Pick the right model for your needs."
			tagColor="bg-accent-pink"
			tagIcon="arrow"
            imageSrc="/generated/image-multiple-ai-model-logos-and-interfaces-d-1765491630802-3.webp"
		/>
		
		<FeatureCard 
			subtitle="[ CODEBASE AWARE ]"
			title="AI that understands<br>your project"
			description="Goji analyzes your entire game project to generate code that fits your style and architecture."
			tagColor="bg-accent-yellow"
			tagIcon="plus"
            imageSrc="/generated/image-game-developer-analyzing-project-files-a-1765491633163-4.webp"
		/>
	</div>
</section>
