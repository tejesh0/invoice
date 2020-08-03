<script>
	import Invoice from '../components/Invoice.svelte';
	import Dashboard from '../components/Dashboard.svelte';
	// export let segment;
</script>

<style>
	main {
		position: relative;
		background-color: white;
		margin: 0 auto;
	}
	.flex-50 {
		flex: 0 0 50%;
		flex-flow: wrap;
	}
</style>

<!-- <Nav {segment}/> -->

<main class="block md:flex">
	<section class="flex-50 p-5 bg-blue-800">
		<Invoice></Invoice>
	</section>
	<section class="p-5 flex-50">
		<Dashboard></Dashboard>
	</section>
</main>
