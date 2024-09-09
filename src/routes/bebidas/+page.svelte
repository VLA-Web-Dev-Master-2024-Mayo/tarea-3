<script lang="ts">
	import Bebidas from "../bebidas.svelte";
</script>

<!-- boton para volver al inicio -->

<div class="flex justify-center items-end gap-2 p-2">
	<a
		href="/"
		class="border-2 bg-yellow-400 border-yellow-600 border-spacing-10 p-1 text-center text-white text-3xl font-bold px-2 rounded-full"
		>Pagina Principal
	</a>
</div>

<!-- restos de bebidas -->

<Bebidas />
