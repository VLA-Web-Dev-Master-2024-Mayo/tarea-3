<script lang="ts">
	import Footer from "$lib/components/Footer.svelte";
	import Burger from "$lib/components/Hamburguesas.svelte";
	import Sidebar from "$lib/components/Sidebar.svelte";
</script>

<!-- <svelte:head>
	<script src="https://cdn.tailwindcss.com"></script>
</svelte:head> -->

<header class="header">
	<a href="/">Inicio</a>
</header>

<main class="main">
	<h1 class="text-red-400">Nuestros productos</h1>
	<Sidebar />
	<Burger />
</main>

<footer>
	<Footer />
</footer>
