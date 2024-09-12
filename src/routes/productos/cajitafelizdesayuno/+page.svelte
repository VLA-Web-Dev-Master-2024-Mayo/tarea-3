<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Menu_items, { type Menu_item as MMenu_item } from "$lib/components/Menu_item.svelte";
	let menu_items_productos: MMenu_item[] = $state([]);
	let menu_items_bebidas: MMenu_item[] = $state([]);
	let menu_items_postres: MMenu_item[] = $state([]);
	menu_items_productos = [
		{
			title: "Pancake con Huevo",
			page_link: "",
			img_src: "/assets/cajitafelizdesayuno/pancakeconhuevo.png",
		},
	];

	menu_items_bebidas = [
		{
			title: "Nectar de Manzana",
			page_link: "",
			img_src: "/assets/cajitafelizdesayuno/nectardemanzana.png",
		},
	];
	menu_items_postres = [
		{
			title: "Yogurt de Fresa",
			page_link: "",
			img_src: "/assets/cajitafelizdesayuno/yogurtdefresa.png",
		},
	];
</script>

<Card title="Cajita Feliz" />
<h2 class="font-bold text-center text-3xl mt-5">Productos</h2>
<Menu_items menu_items={menu_items_productos} />
<h2 class="font-bold text-center text-3xl mt-5">Bebidas</h2>
<Menu_items menu_items={menu_items_bebidas} />
<h2 class="font-bold text-center text-3xl mt-5">Postres</h2>
<Menu_items menu_items={menu_items_postres} />
