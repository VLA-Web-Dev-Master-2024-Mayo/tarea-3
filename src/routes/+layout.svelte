<script lang="ts">
	import Footer from "$lib/components/Footer.svelte";
	import Navbar from "$lib/components/Navbar.svelte";
</script>

<header class="header">
	<Navbar />
</header>
<main>
	<slot />
</main>

<footer>
	<Footer />
</footer>

<style>
	.header {
		display: flex;
		height: 10rem; /* 48 en Tailwind es 12rem */
		background-color: white;
		width: 100%;
		position: fixed;
		top: 0;
		z-index: 1000;
	}

	main {
		margin-top: 10rem;
		position: relative;
		z-index: 0;
	}
</style>
