<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Menu_items, { type Menu_item as MMenu_item } from "$lib/components/Menu_item.svelte";
	let menu_items_productos: MMenu_item[] = $state([]);
	let menu_items_acompanamientos: MMenu_item[] = $state([]);
	let menu_items_bebidas: MMenu_item[] = $state([]);
	let menu_items_postres: MMenu_item[] = $state([]);
	menu_items_productos = [
		{
			title: "McNuggets 4 unidades (Cajita Feliz)",
			page_link: "",
			img_src: "/assets/cajitafeliz/productos/mcnuggets4und(cajitasfeliz).png",
		},
		{
			title: "Pieza de Pollo (Cajita Feliz)",
			page_link: "",
			img_src: "/assets/cajitafeliz/productos/piezadepollo(cajitafeliz).png",
		},
		{
			title: "Hamburguesa (Cajita Feliz)",
			page_link: "",
			img_src: "/assets/cajitafeliz/productos/hamburguesacajitafeliz.png",
		},
		{
			title: "Mac Fiesta Jr (Cajita Feliz)",
			page_link: "",
			img_src: "/assets/cajitafeliz/productos/mcfiestajr(cajitafeliz).png",
		},
	];
	menu_items_acompanamientos = [
		{
			title: "Papas Kids (Cajita Feliz)",
			page_link: "",
			img_src: "/assets/cajitafeliz/acompanamientos/papaskids(cajitafeliz).png",
		},
	];
	menu_items_bebidas = [
		{
			title: "Agua Embotellada",
			page_link: "",
			img_src: "/assets/cajitafeliz/bebidas/aguaembotellada(cajitafeliz).png",
		},
		{
			title: "Nectar de Manzana",
			page_link: "",
			img_src: "/assets/cajitafeliz/bebidas/nectardemanzana(cajitafeliz).png",
		},
	];
	menu_items_postres = [
		{
			title: "Yogurt de Fresa",
			page_link: "",
			img_src: "/assets/cajitafeliz/postres/yogurtdefresa(cajitafeliz).png",
		},
	];
</script>

<Card title="Cajita Feliz" />
<h2 class="font-bold text-center text-3xl mt-5">Productos</h2>
<Menu_items menu_items={menu_items_productos} />
<h2 class="font-bold text-center text-3xl mt-5">Acompnamientos</h2>
<Menu_items menu_items={menu_items_acompanamientos} />
<h2 class="font-bold text-center text-3xl mt-5">Bebidas</h2>
<Menu_items menu_items={menu_items_bebidas} />
<h2 class="font-bold text-center text-3xl mt-5">Postres</h2>
<Menu_items menu_items={menu_items_postres} />
