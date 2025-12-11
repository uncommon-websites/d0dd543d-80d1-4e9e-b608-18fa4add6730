<script lang="ts">
	import { slide } from 'svelte/transition';

	const faqs = [
		{
			question: "How does Goji pricing work?",
			answer: "Goji uses a credit-based system. Credits are consumed based on your prompt length and generated output. We offer three tiers: Hobby (free, 100 credits), Indie ($20/month, 3,000 credits), and Studio ($40/user/month, 6,000 credits per seat)."
		},
		{
			question: "Does Goji only work with Godot?",
			answer: "Yes, Goji is specifically designed for Godot game development. It generates GDScript code and understands Godot's scene system and architecture."
		},
		{
			question: "Do I own the code that Goji generates?",
			answer: "Absolutely! You own all code generated using Goji. There are no IP claims by us on your content, and you can use it commercially without any restrictions."
		},
		{
			question: "Which AI models does Goji support?",
			answer: "Goji supports multiple AI models including Claude, Gemini, and other top models. You can choose different models for different tasks from a single interface."
		},
		{
			question: "Is Goji available on Linux?",
			answer: "Currently, Goji is available for macOS and Windows. Linux support is on our roadmap based on community demand."
		},
		{
			question: "Does Goji require an internet connection?",
			answer: "Yes, Goji needs internet to access AI models. However, your project files stay local on your machine—we don't upload or store your game code."
		},
		{
			question: "Can I use Goji for commercial games?",
			answer: "Yes! All code generated with Goji can be used in commercial projects. You retain full ownership and rights to everything you create."
		}
	];

	let openIndex: number | null = null;

	function toggle(index: number) {
		openIndex = openIndex === index ? null : index;
	}
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto border-t border-gray-200">
	<div class="grid grid-cols-1 lg:grid-cols-3 gap-12">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ FAQ ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-6">
				Frequently Asked Questions
			</h2>
			<p class="font-mono text-sm text-gray-600 mb-8">
				Your question not answered here?
			</p>
			<button class="bg-primary-600 text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-primary-700 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
				<svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
				Contact Us
			</button>
		</div>

		<div class="lg:col-span-2 space-y-4">
			{#each faqs as faq, i}
				<div class="border-b border-gray-200 pb-4">
					<button class="w-full flex items-center justify-between text-left py-2 group" on:click={() => toggle(i)}>
						<span class="font-mono text-sm font-medium text-gray-800 group-hover:text-primary-600 transition-colors pr-8">{faq.question}</span>
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-400 transition-transform duration-300 {openIndex === i ? 'rotate-180' : ''}"><path d="m6 9 6 6 6-6"/></svg>
					</button>
					{#if openIndex === i}
						<div transition:slide={{ duration: 300 }} class="overflow-hidden">
							<p class="pt-2 pb-4 text-sm text-gray-600 leading-relaxed max-w-2xl font-mono">
								{faq.answer}
							</p>
						</div>
					{/if}
				</div>
			{/each}
		</div>
	</div>
</section>
