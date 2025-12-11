<script lang="ts">
	const testimonials = [
		{
			quote: "I shipped my first game in 3 weeks thanks to Goji. As a solo dev with limited coding skills, this is exactly what I needed to bring my ideas to life.",
			author: "Alex Chen",
			role: "Indie Dev • Pixel Dreams",
			image: "https://i.pravatar.cc/150?u=alex",
            icon: "https://placehold.co/20x20/D97706/fff?text=G"
		},
		{
			quote: "Goji understands Godot better than any AI tool I've tried. It generates clean GDScript that actually works with my project structure.",
			author: "Sarah Martinez",
			role: "Solo Developer",
			image: "https://i.pravatar.cc/150?u=sarah",
            icon: "https://placehold.co/20x20/D97706/fff?text=G"
		},
		{
			quote: "Finally, an AI tool made for game devs. I can describe a mechanic in plain English and Goji builds it. Game-changer for prototyping.",
			author: "Jake Thompson",
			role: "Game Designer • Moonlight Studios",
			image: "https://i.pravatar.cc/150?u=jake",
            icon: "https://placehold.co/20x20/D97706/fff?text=G"
		},
		{
			quote: "The scene builder is incredible. I described my level layout and Goji created the entire node structure. Saved me hours of tedious work.",
			author: "Priya Patel",
			role: "Indie Developer",
			image: "https://i.pravatar.cc/150?u=priya",
            icon: "https://placehold.co/20x20/D97706/fff?text=G"
		},
		{
			quote: "I'm not a programmer, I'm a designer. Goji lets me focus on game design while it handles the code. This is the future of indie game dev.",
			author: "Marcus Johnson",
			role: "Game Designer",
			image: "https://i.pravatar.cc/150?u=marcus",
            icon: "https://placehold.co/20x20/D97706/fff?text=G"
		},
		{
			quote: "Switched from Unity to Godot and Goji made the transition smooth. It helped me learn GDScript while building my game at the same time.",
			author: "Emma Wilson",
			role: "Solo Dev • Starlight Games",
			image: "https://i.pravatar.cc/150?u=emma",
            icon: "https://placehold.co/20x20/D97706/fff?text=G"
		},
        {
			quote: "The multi-model support is brilliant. I use Claude for complex game logic and Gemini for creative content. Having both in one tool is perfect.",
			author: "David Kim",
			role: "Indie Developer",
			image: "https://i.pravatar.cc/150?u=david",
            icon: "https://placehold.co/20x20/D97706/fff?text=G"
		},
        {
			quote: "Goji paid for itself in the first week. What used to take me days now takes hours. Can't imagine going back to coding everything manually.",
			author: "Lisa Rodriguez",
			role: "Solo Game Developer",
			image: "https://i.pravatar.cc/150?u=lisa",
            icon: "https://placehold.co/20x20/D97706/fff?text=G"
		}
	];
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ TESTIMONIALS ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-4">
			Loved by Indie Developers
		</h2>
		<p class="font-mono text-sm text-gray-600">
			See what game developers are saying about building with Goji
		</p>
	</div>

	<div class="columns-1 md:columns-2 lg:columns-3 gap-6 space-y-6">
		{#each testimonials as t}
			<div class="bg-white p-6 rounded-lg border border-gray-200 shadow-sm break-inside-avoid hover:shadow-md transition-shadow">
				<p class="font-mono text-xs leading-relaxed text-gray-700 mb-6">
					"{t.quote}"
				</p>
				<div class="flex items-center justify-between border-t border-gray-100 pt-4">
					<div class="flex items-center gap-3">
						<img src={t.image} alt={t.author} class="w-8 h-8 rounded-full bg-gray-200" />
						<div>
							<div class="text-xs font-bold text-gray-900">{t.author}</div>
							<div class="text-[10px] text-gray-500 font-mono">{t.role}</div>
						</div>
					</div>
                    <img src={t.icon} alt="Company Logo" class="w-5 h-5 rounded-sm opacity-70 grayscale" />
				</div>
			</div>
		{/each}
	</div>
</section>
