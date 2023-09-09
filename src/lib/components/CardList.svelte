<script lang="ts">
	export let items: string[];
</script>

<ul class="space-y-4 mb-8">
	{#each items as item}
		<li
			class="px-4 py-4 flex items-center justify-center rounded border-4 border-black cursor-pointer select-none active:scale-95"
		>
			{item}
		</li>
	{/each}
</ul>
<div class="text-base italic text-center">Maybe more later.</div>
