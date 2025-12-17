<section class="py-20 border-b border-border">
	<div class="container-custom">
		<div class="grid grid-cols-1 md:grid-cols-2 gap-16">
			
			<!-- Left Column: CTA & Visual -->
			<div class="flex flex-col h-full">
				<div class="mb-8">
					<p class="font-mono text-xs text-muted mb-4">Start building</p>
					<h2 class="text-2xl font-medium mb-4">Scale to 100K agents with confidence</h2>
					<p class="text-muted font-light mb-8 text-sm leading-relaxed max-w-md">
						AI Agent Builder helps product teams at AI companies deliver consistent, reliable agent outputs through optimized prompt engineering.
					</p>
					<div class="flex gap-3 mb-12">
						<button class="border border-border px-3 py-1.5 text-xs font-mono uppercase hover:bg-primary-50 transition-colors flex items-center gap-2">
							START FREE TRIAL
							<span class="text-muted border border-muted/30 rounded px-1 text-[9px] min-w-[16px] text-center">S</span>
						</button>
						<button class="border border-border px-3 py-1.5 text-xs font-mono uppercase hover:bg-primary-50 transition-colors flex items-center gap-2">
							VIEW TEMPLATES
							<span class="text-muted border border-muted/30 rounded px-1 text-[9px] min-w-[16px] text-center">T</span>
						</button>
					</div>
				</div>
				
				<!-- Barcode Visual -->
				<div class="mt-auto w-full h-48 bg-black relative overflow-hidden flex items-center justify-center">
					{#each Array(100) as _, i}
						<div 
							class="h-full bg-white absolute" 
							style="
								left: {i}%; 
								width: {Math.random() * 2}%; 
								opacity: {Math.random()};
							"
						></div>
					{/each}
					<div class="absolute inset-0 flex items-center justify-center">
						<div class="bg-black text-white font-mono text-[10px] px-2 py-1 z-10">
							agentbuilder.ai
						</div>
					</div>
				</div>
			</div>

			<!-- Right Column: Updates -->
			<div>
				<p class="font-mono text-xs text-muted mb-8">Latest updates</p>
				
				<div class="space-y-12">
					<!-- Update 1 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">January 15</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Launching Template Marketplace</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								Our new Template Marketplace features 50+ battle-tested prompt templates for common agent tasks. Each template includes consistency scores, usage examples, and customization guides. Templates cover customer support, data extraction, content generation, code review, and more. Start building production-ready agents in minutes, not hours.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Product Release</span>
						</div>
					</div>

					<!-- Update 2 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">January 8</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">AI Agent Builder achieves 94% consistency score</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								New benchmark results show AI Agent Builder delivers 94% output consistency across 500 real-world agent tasks, 3x better than manual prompting and 40% better than competitors. Our optimization engine reduces engineering time by 80% while improving agent reliability.
							</p>
							<div class="flex gap-2">
								<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Benchmarks</span>
								<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Research</span>
							</div>
						</div>
					</div>

					<!-- Update 3 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">December 20</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Introducing Team Collaboration Features</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								Share prompts across teams, set granular permissions, and maintain complete audit logs. New enterprise features include SSO integration, custom roles, and compliance reporting. Perfect for product teams scaling to hundreds of agents.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Product Release</span>
						</div>
					</div>

					<!-- Update 4 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">December 1</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Preparing for Product Hunt launch</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								We're launching on Product Hunt this month! Join our waitlist to get early access, exclusive templates, and founding member pricing. Help us bring consistent AI agent outputs to product teams everywhere.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Announcement</span>
						</div>
					</div>
				</div>
			</div>

		</div>
	</div>
</section>
