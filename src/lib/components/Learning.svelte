<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto relative overflow-hidden">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ DESKTOP APP ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-6 leading-[0.95]">
				Works right in<br>your workflow.
			</h2>
			<p class="font-mono text-sm text-gray-600 max-w-md mb-8 leading-relaxed">
				Goji is a native desktop app for macOS and Windows. No browser tabs, no context switching. Just you, your Godot project, and AI assistance when you need it.
			</p>
			
			<button class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs w-fit">
				<span class="text-primary-400">✦</span> Download Now
			</button>
		</div>

		<div class="relative h-[400px] w-full flex items-center justify-center">
			<!-- Background Text Pattern -->
            <div class="absolute inset-0 flex flex-col items-center justify-center opacity-5 select-none pointer-events-none overflow-hidden leading-none">
                {#each Array(10) as _, i}
                    <div class="text-6xl md:text-8xl font-black text-gray-900 whitespace-nowrap">
                        GOJI GOJI GOJI GOJI
                    </div>
                {/each}
            </div>

            <!-- Floating Cards -->
            <div class="relative z-10 flex flex-col gap-4 w-full max-w-md">
                <div class="bg-white p-4 rounded shadow-lg border border-gray-200 transform -rotate-2 translate-x-4">
                    <div class="flex items-center gap-2 mb-2">
                        <span class="bg-primary-600 text-white text-[10px] font-bold px-1.5 py-0.5 rounded uppercase">Generated</span>
                        <span class="text-xs text-gray-500">Just now</span>
                    </div>
                    <p class="text-sm font-mono text-gray-800">Created player movement script with jump mechanics</p>
                </div>

                <div class="bg-white p-4 rounded shadow-lg border border-gray-200 transform rotate-1 translate-x-8">
                    <div class="flex items-center gap-2 mb-2">
                        <span class="bg-primary-600 text-white text-[10px] font-bold px-1.5 py-0.5 rounded uppercase">Generated</span>
                        <span class="text-xs text-gray-500">5m ago</span>
                    </div>
                    <p class="text-sm font-mono text-gray-800">Built enemy AI scene with patrol behavior</p>
                </div>

                 <div class="bg-white p-4 rounded shadow-lg border border-gray-200 transform -rotate-1">
                    <div class="flex items-center gap-2 mb-2">
                        <span class="bg-primary-600 text-white text-[10px] font-bold px-1.5 py-0.5 rounded uppercase">Generated</span>
                        <span class="text-xs text-gray-500">12m ago</span>
                    </div>
                    <p class="text-sm font-mono text-gray-800">Added inventory system with item pickup</p>
                </div>
            </div>
		</div>
	</div>
</section>
