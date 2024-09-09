<script lang="ts">
	import Hamburguesa from "../hamburguesa.svelte";
</script>

<!-- Boton para volver al inicio -->

<div class="flex justify-center items-end gap-2 p-2">
	<a
		href="/"
		class="border-2 bg-stone-700 border-white border-spacing-10 p-1 text-center text-white text-3xl font-bold px-2 rounded-full"
		>Pagina Principal
	</a>
</div>

<!-- distintas hamburguesas -->

<Hamburguesa />
