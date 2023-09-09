<script lang="ts">
	export let items: ListItem[];

	const openItem = (item: ListItem) => {
		window.open(item.link);
	};
</script>

<ul class="space-y-4 mb-8">
	{#each items as item}
		<li>
			<button
				class="px-4 py-4 flex items-center justify-center w-full rounded border-4 border-black cursor-pointer select-none active:scale-95"
				on:click={() => openItem(item)}
			>
				{item.name}
			</button>
		</li>
	{/each}
</ul>
<div class="text-base italic text-center">Maybe more later.</div>
