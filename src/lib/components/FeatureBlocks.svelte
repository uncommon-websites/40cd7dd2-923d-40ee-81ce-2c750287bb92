<script lang="ts">
	import FeatureBlock from './FeatureBlock.svelte';
</script>

<!-- Block 1: Pre-built Templates -->
<FeatureBlock 
	title="Pre-built prompt templates" 
	description="Start with battle-tested templates for common agent tasks. Customize for your use case in minutes."
	buttons={[
		{ text: "BROWSE TEMPLATES", icon: true },
		{ text: "LEARN MORE" }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm p-4 font-mono text-xs">
		<div class="flex items-center gap-2 border-b border-border pb-2 mb-4">
			<span class="text-accent">📋</span>
			<span class="text-muted">Customer Support Agent</span>
		</div>
		<div class="space-y-3">
			<div class="flex items-center gap-2">
				<div class="w-2 h-2 bg-green-500 rounded-full"></div>
				<span class="text-gray-600">94% consistency</span>
			</div>
			<div class="h-2 bg-gray-100 w-3/4 rounded"></div>
			<div class="h-2 bg-gray-100 w-5/6 rounded"></div>
			<div class="h-2 bg-gray-100 w-2/3 rounded"></div>
		</div>
	</div>
</FeatureBlock>

<!-- Block 2: AI-Powered Optimization -->
<FeatureBlock 
	title="AI-powered prompt optimization" 
	description="Transform vague instructions into precise, production-ready prompts instantly with our optimization engine."
	buttons={[
		{ text: "TRY OPTIMIZER", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full max-w-md bg-white border border-border rounded shadow-sm p-6 flex flex-col gap-4">
		<div class="flex items-center gap-2 text-xs font-mono text-muted">
			<div class="w-4 h-4 border border-current rounded-sm flex items-center justify-center">
				<div class="w-2 h-2 bg-current rounded-[1px]"></div>
			</div>
			Optimizing prompt...
		</div>
		<div class="w-full bg-gray-100 h-1.5 rounded-full overflow-hidden">
			<div class="bg-accent h-full w-2/3 transition-all"></div>
		</div>
		<div class="flex gap-1">
			{#each Array(20) as _, i}
				<div class="w-1 h-3 {i < 14 ? 'bg-accent/30' : 'bg-gray-200'}"></div>
			{/each}
		</div>
		<div class="mt-2 flex items-center gap-2 text-[10px] text-muted font-mono uppercase">
			<span class="w-3 h-3 border border-current rounded-full flex items-center justify-center">✓</span>
			OPTIMIZED
		</div>
	</div>
</FeatureBlock>

<!-- Block 3: Version Control & Testing -->
<FeatureBlock 
	title="Version control & A/B testing" 
	description="Track every prompt change, test variations side-by-side, and roll back instantly when needed."
	buttons={[
		{ text: "VIEW VERSIONS", icon: true }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm overflow-hidden font-mono text-[10px]">
		<div class="grid grid-cols-4 gap-2 p-2 border-b border-border bg-gray-50 text-muted">
			<div>VERSION</div>
			<div>CONSISTENCY</div>
			<div>ACCURACY</div>
			<div>STATUS</div>
		</div>
		{#each [
			{ v: 'v2.4', c: '94%', a: '98%', s: 'PROD' },
			{ v: 'v2.3', c: '91%', a: '97%', s: 'TEST' },
			{ v: 'v2.2', c: '88%', a: '96%', s: 'ARCHIVED' },
			{ v: 'v2.1', c: '85%', a: '95%', s: 'ARCHIVED' },
			{ v: 'v2.0', c: '82%', a: '94%', s: 'ARCHIVED' },
			{ v: 'v1.9', c: '79%', a: '93%', s: 'ARCHIVED' }
		] as row}
			<div class="grid grid-cols-4 gap-2 p-2 border-b border-border/50 items-center">
				<div class="text-blue-600">{row.v}</div>
				<div class="text-muted">{row.c}</div>
				<div class="text-muted">{row.a}</div>
				<div class="text-[9px] {row.s === 'PROD' ? 'text-green-600' : 'text-gray-400'}">{row.s}</div>
			</div>
		{/each}
	</div>
</FeatureBlock>

<!-- Block 4: Team Collaboration -->
<FeatureBlock 
	title="Team collaboration & access control" 
	description="Share prompts across teams, set permissions, and maintain audit logs for enterprise compliance."
	buttons={[
		{ text: "INVITE TEAM", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm overflow-hidden font-mono text-[10px]">
		<div class="grid grid-cols-4 gap-2 p-2 border-b border-border bg-gray-50 text-muted">
			<div>MEMBER</div>
			<div>ROLE</div>
			<div>PROMPTS</div>
			<div>ACCESS</div>
		</div>
		{#each [
			{ name: 'Sarah Chen', role: 'Admin', prompts: '24', access: 'Full' },
			{ name: 'Mike Ross', role: 'Editor', prompts: '18', access: 'Edit' },
			{ name: 'Emma Liu', role: 'Editor', prompts: '12', access: 'Edit' },
			{ name: 'James Park', role: 'Viewer', prompts: '8', access: 'View' },
			{ name: 'Lisa Wang', role: 'Viewer', prompts: '5', access: 'View' },
			{ name: 'Tom Davis', role: 'Viewer', prompts: '3', access: 'View' }
		] as member}
			<div class="grid grid-cols-4 gap-2 p-2 border-b border-border/50 items-center">
				<div class="flex items-center gap-2">
					<div class="w-3 h-3 rounded-full bg-indigo-400/20"></div>
					<span class="text-indigo-600">{member.name}</span>
				</div>
				<div class="text-muted">{member.role}</div>
				<div class="text-muted">{member.prompts}</div>
				<div class="text-[9px] text-gray-400">{member.access}</div>
			</div>
		{/each}
	</div>
</FeatureBlock>

<!-- Block 5: Performance Analytics -->
<FeatureBlock 
	title="Real-time performance analytics" 
	description="Monitor agent outputs, track consistency scores, and identify optimization opportunities automatically."
	buttons={[
		{ text: "VIEW ANALYTICS", icon: true }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm p-4 flex flex-col gap-4">
		<div class="flex items-center justify-between border-b border-border pb-2">
			<div class="text-[10px] font-mono text-muted flex items-center gap-2">
				<span class="w-2 h-2 bg-green-500 rounded-full"></span>
				Last 30 days performance
			</div>
		</div>
		
		<!-- Performance Grid visual -->
		<div class="grid grid-cols-12 gap-1">
			{#each Array(48) as _, i}
				<div class="aspect-square rounded-[1px] {i > 40 ? 'bg-green-500' : i > 30 ? 'bg-green-400' : i > 20 ? 'bg-green-300' : i > 10 ? 'bg-green-200' : 'bg-gray-100'}"></div>
			{/each}
		</div>

		<div class="mt-auto space-y-2">
			<div class="flex items-center gap-2 text-[10px] text-muted font-mono">
				<span class="w-3 h-3 border border-current rounded-full flex items-center justify-center text-[8px]">↑</span>
				+12% consistency
			</div>
			<div class="bg-green-50 p-2 rounded border border-green-200 flex gap-2 items-center">
				<div class="w-4 h-4 bg-green-500 rounded flex items-center justify-center text-white text-[8px]">✓</div>
				<div class="text-[10px] text-green-700">All agents performing well</div>
			</div>
		</div>
	</div>
</FeatureBlock>
