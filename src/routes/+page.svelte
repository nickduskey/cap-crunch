<script lang="ts">
	import * as Card from '$lib/components/ui/card';
	import Signings from '$lib/components/tables/Signings.svelte';
</script>

<div class="flex items-center justify-between space-y-2">
	<h2 class="text-3xl font-bold tracking-tight">Home</h2>
	<div class="grid gap-4 md:grid-cols-2 lg:grid-cols-4">
		<Card.Root>
			<Card.Header>
				<Card.Title>Signings</Card.Title>
			</Card.Header>
			<Card.Content>
				<Signings />
			</Card.Content>
		</Card.Root>
	</div>
</div>
