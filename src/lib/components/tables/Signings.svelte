<script lang="ts">
	import * as Table from '$lib/components/ui/table/index';

	interface Signing {
		icon: string;
		name: string;
		capHit: number;
	}

	const signings: Signing[] = [
		{
			icon: '/icons/stl.svg',
			name: 'Colten Ellis',
			capHit: 775000
		},
		{
			icon: '/icons/stl.svg',
			name: 'Mathias Leferriere',
			capHit: 775000
		},
		{
			icon: '/icons/tbl.svg',
			name: 'Decian Carlile',
			capHit: 775000
		},
		{
			icon: '/icons/lak.svg',
			name: 'Akil Thomas',
			capHit: 775000
		},
		{
			icon: '/icons/lak.svg',
			name: 'Andre Lee',
			capHit: 775000
		},
		{
			icon: '/icons/mtl.svg',
			name: 'Connor Hughes',
			capHit: 775000
		},
		{
			icon: '/icons/det.svg',
			name: 'Jakub Rychlovsky',
			capHit: 870000
		},
		{
			icon: '/icons/ana.svg',
			name: 'Damian Clara',
			capHit: 878333
		}
	];
</script>

<Table.Root>
	<Table.Caption>A list of recent signings.</Table.Caption>
	<Table.Header>
		<Table.Row>
			<Table.Head>Player</Table.Head>
			<Table.Head>Cap Hit</Table.Head>
		</Table.Row>
	</Table.Header>
	<Table.Body>
		{#each signings as signing, i (i)}
			<Table.Row>
				<Table.Cell>{signing.name}</Table.Cell>
				<Table.Cell class="text-right">{signing.capHit}</Table.Cell>
			</Table.Row>
		{/each}
	</Table.Body>
</Table.Root>
