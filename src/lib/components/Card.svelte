<!-- <script lang="ts" module>
	export type Item = { title: string };
</script>
 -->
<script lang="ts">
	type Props = { title: string };
	const { title }: Props = $props();
</script>

<div class="relative text-center ml-10 mt-[200px]">
	<div class="flex gap-1">
		<i class="bi bi-house"></i>
		<a href="/" class="text-base underline text-blue-700 decoration-blue-700">Inicio</a>
		<span class="text-gray-500">&gt;</span>
		<a href="/productos" class="underline text-blue-700 decoration-blue-700">Productos</a>
		<span class="text-gray-500">&gt;</span>
		<span class="text-gray-500">{title}</span>
	</div>
	<h1 class="text-[3rem] font-extrabold">{title}</h1>
</div>
