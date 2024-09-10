<script lang="ts">
	import Footer from "$lib/components/Footer.svelte";

	import Navbar from "$lib/components/Navbar.svelte";
</script>

<header class="header">
	<Navbar />
</header>

<main class="main">
	<img src="/assets/portada.jpg" alt="Imagen de portada" />
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
		z-index: 1000; /* Asegura que esté sobre el main */
	}

	.main {
		margin-top: 10rem; /* Asegura que el main comience después del header */
		position: relative;
		z-index: 0;
	}

	.main img {
		width: 100%;
		height: auto;
		position: relative;
	}
</style>
