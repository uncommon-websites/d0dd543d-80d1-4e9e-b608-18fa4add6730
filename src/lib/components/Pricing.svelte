<script lang="ts">
	const plans = [
		{
			name: 'Hobby',
			price: '$0',
			period: 'forever',
			credits: '100 credits/month',
			description: 'Perfect for trying out Goji',
			features: [
				'100 credits per month',
				'Access to all AI models',
				'Basic support',
				'Community access',
				'Desktop app (macOS & Windows)'
			],
			cta: 'Start Free',
			popular: false
		},
		{
			name: 'Indie',
			price: '$20',
			period: 'per month',
			credits: '3,000 credits/month',
			description: 'For solo developers shipping games',
			features: [
				'3,000 credits per month',
				'Access to all AI models',
				'Priority support',
				'Community access',
				'Desktop app (macOS & Windows)',
				'Early access to new features'
			],
			cta: 'Get Started',
			popular: true
		},
		{
			name: 'Studio',
			price: '$40',
			period: 'per user/month',
			credits: '6,000 credits/seat',
			description: 'For small teams building together',
			features: [
				'6,000 credits per seat',
				'Access to all AI models',
				'Priority support',
				'Team billing',
				'Admin dashboard',
				'Usage analytics',
				'Dedicated account manager'
			],
			cta: 'Contact Sales',
			popular: false
		}
	];
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto" id="pricing">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ PRICING ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-4">
			Simple, credit-based pricing
		</h2>
		<p class="font-mono text-sm text-gray-600 max-w-2xl mx-auto">
			Pay only for what you use. Credits scale with prompt and output length. No hidden fees.
		</p>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-6xl mx-auto">
		{#each plans as plan}
			<div class="bg-white rounded-lg border-2 {plan.popular ? 'border-primary-600' : 'border-gray-200'} p-8 relative flex flex-col hover:shadow-lg transition-shadow">
				{#if plan.popular}
					<div class="absolute -top-3 left-1/2 -translate-x-1/2 bg-primary-600 text-white px-4 py-1 rounded-full text-xs font-mono uppercase tracking-wider">
						Most Popular
					</div>
				{/if}

				<div class="mb-6">
					<h3 class="font-display text-2xl font-medium mb-2">{plan.name}</h3>
					<div class="flex items-baseline gap-2 mb-2">
						<span class="font-display text-5xl font-medium">{plan.price}</span>
						<span class="text-sm text-gray-500 font-mono">{plan.period}</span>
					</div>
					<p class="text-xs text-gray-600 font-mono mb-4">{plan.credits}</p>
					<p class="text-sm text-gray-600">{plan.description}</p>
				</div>

				<ul class="space-y-3 mb-8 flex-grow">
					{#each plan.features as feature}
						<li class="flex items-start gap-2 text-sm text-gray-700">
							<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-primary-600 shrink-0 mt-0.5"><path d="M20 6 9 17l-5-5"/></svg>
							<span>{feature}</span>
						</li>
					{/each}
				</ul>

				<button class="w-full {plan.popular ? 'bg-primary-600 hover:bg-primary-700' : 'bg-black hover:bg-gray-800'} text-white py-3 rounded text-sm font-medium transition-colors font-mono uppercase tracking-wide">
					{plan.cta}
				</button>
			</div>
		{/each}
	</div>

	<div class="mt-16 text-center">
		<p class="text-sm text-gray-600 font-mono mb-4">
			Need a custom plan? <a href="#" class="text-primary-600 hover:underline">Contact us</a>
		</p>
		<div class="flex items-center justify-center gap-8 text-xs text-gray-500 font-mono">
			<span>✓ No credit card required</span>
			<span>✓ Cancel anytime</span>
			<span>✓ All plans include full feature access</span>
		</div>
	</div>
</section>
