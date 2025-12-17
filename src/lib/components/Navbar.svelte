<script lang="ts">
	import { onMount } from 'svelte';
	
	let showBanner = true;
</script>

{#if showBanner}
	<div class="bg-primary-50 border-b border-border py-2 px-4 text-xs font-mono flex justify-center items-center relative">
		<div class="flex items-center gap-2">
			<span class="text-muted">Launching on Product Hunt this month.</span>
			<a href="#" class="underline decoration-muted hover:text-accent transition-colors">Get notified.</a>
		</div>
		<button 
			class="absolute right-4 text-muted hover:text-foreground"
			aria-label="Close banner"
			onclick={() => showBanner = false}
		>
			<svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
				<path d="M9 3L3 9M3 3L9 9" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
			</svg>
		</button>
	</div>
{/if}

<nav class="border-b border-border bg-background sticky top-0 z-50">
	<div class="container-custom h-16 flex items-center justify-between">
		<!-- Logo -->
		<a href="/" class="text-xl font-bold tracking-tight flex items-center gap-2">
			<svg width="24" height="13" viewBox="0 0 116 63" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-foreground">
				<path d="M115.364 0H74.4491C71.5379 0 68.7844 1.32346 66.9657 3.59662L63.1372 8.38254C61.3185 10.6557 58.5649 11.9792 55.6538 11.9792H19.5306L9.94727 23.9583H50.8621C53.7733 23.9583 56.5268 22.6349 58.3455 20.3617L62.174 15.5758C63.9927 13.3026 66.7462 11.9792 69.6574 11.9792H105.781L115.364 0Z" fill="currentColor"/>
				<path d="M110.571 19.1665H69.6561C66.7449 19.1665 63.9914 20.49 62.1727 22.7631L58.3442 27.549C56.5255 29.8222 53.772 31.1457 50.8608 31.1457H14.7376L5.1543 43.1248H46.0691C48.9803 43.1248 51.7338 41.8014 53.5525 39.5282L57.3811 34.7423C59.1997 32.4691 61.9533 31.1457 64.8645 31.1457H100.988L110.571 19.1665Z" fill="currentColor"/>
				<path d="M105.78 38.3333H64.8651C61.9539 38.3333 59.2004 39.6567 57.3817 41.9299L53.5532 46.7158C51.7345 48.989 48.981 50.3124 46.0698 50.3124H9.94661L0.363281 62.2916H41.2781C44.1893 62.2916 46.9428 60.9681 48.7615 58.695L52.59 53.909C54.4087 51.6359 57.1623 50.3124 60.0734 50.3124H96.1966L105.78 38.3333Z" fill="currentColor"/>
			</svg>
			<span class="font-sans font-semibold">AI Agent Builder</span>
		</a>

		<!-- Links -->
		<div class="hidden md:flex items-center gap-8 font-mono text-xs text-muted">
			<a href="#" class="hover:text-foreground transition-colors">Templates</a>
			<a href="#" class="hover:text-foreground transition-colors">Pricing</a>
			<a href="#" class="hover:text-foreground transition-colors">Blog</a>
			<a href="#" class="hover:text-foreground transition-colors">Docs</a>
		</div>

		<!-- CTA -->
		<div class="flex items-center gap-4">
			<a href="#" class="hidden md:flex items-center gap-2 border border-border px-3 py-1.5 text-xs font-mono hover:bg-primary-50 transition-colors uppercase">
				Start Building
				<svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
					<path d="M1 11L11 1M11 1H3M11 1V9" stroke="currentColor" stroke-width="1.5"/>
				</svg>
			</a>
			<div class="md:hidden">
				<!-- Mobile Menu Icon -->
				<svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
					<line x1="3" y1="12" x2="21" y2="12"></line>
					<line x1="3" y1="6" x2="21" y2="6"></line>
					<line x1="3" y1="18" x2="21" y2="18"></line>
				</svg>
			</div>
		</div>
	</div>
</nav>
