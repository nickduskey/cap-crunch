<script lang="ts">
	import '../app.css';
	import Logo from '$lib/components/Logo.svelte';
	import MainNav from '$lib/components/nav/MainNav.svelte';
	import Search from '$lib/components/nav/Search.svelte';
	import UserNav from '$lib/components/nav/UserNav.svelte';
</script>

<div class="flex-col md:flex">
	<div class="border-b">
		<div class="flex h-16 items-center px-4">
			<Logo />
			<MainNav />
			<div class="ml-auto flex items-center space-x-4">
				<Search />
				<UserNav />
			</div>
		</div>
	</div>
	<div class="flex-1 space-y-4 p-8 pt-6">
		<slot />
	</div>
</div>

<style></style>
