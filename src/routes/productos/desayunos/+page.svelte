<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Menu_items, { type Menu_item as MMenu_item } from "$lib/components/Menu_item.svelte";
	let menu_items: MMenu_item[] = $state([]);

	menu_items = [
		{
			title: "Egg McMuffin",
			page_link: "",
			img_src: "/assets/desayunos/eggmcmuffin.png",
		},
		{
			title: "McMuffin con Salchicha",
			page_link: "",
			img_src: "/assets/desayunos/mcmuffinconsalchicha.png",
		},
		{
			title: "McMuffin Salchicha y Huevo",
			page_link: "",
			img_src: "/assets/desayunos/mcmuffinconsalchichayhuevo.png",
		},
		{
			title: "Huevos Revueltos con Salchicha y Muffin",
			page_link: "",
			img_src: "/assets/desayunos/huevosrevueltosconsalchichaymuffin.png",
		},
		{
			title: "McPinto",
			page_link: "",
			img_src: "/assets/desayunos/mcpinto.png",
		},
		{
			title: "McPinto con Huevo",
			page_link: "",
			img_src: "/assets/desayunos/mcpintoconhuevo.png",
		},
		{
			title: "McPinto Deluxe",
			page_link: "",
			img_src: "/assets/ensaladas/ensaladajardinera.png",
		},
		{
			title: "Pancake",
			page_link: "",
			img_src: "/assets/desayunos/pancake.png",
		},
		{
			title: "Pancake con Salchicha",
			page_link: "",
			img_src: "/assets/desayunos/pancakeconsalchicha.png",
		},
		{
			title: "Derretido",
			page_link: "",
			img_src: "/assets/desayunos/derretido.png",
		},
		{
			title: "Pancake con Huevo",
			page_link: "",
			img_src: "/assets/desayunos/pancakeconhuevo.png",
		},
		{
			title: "Empanada de Carne",
			page_link: "",
			img_src: "/assets/desayunos/empnadadecarne.png",
		},
		{
			title: "Trenza de Jamon y Queso",
			page_link: "",
			img_src: "/assets/desayunos/trenzdejamonyqueso.png",
		},
		{
			title: "Trenza de Pollo",
			page_link: "",
			img_src: "/assets/desayunos/trenzadepollo.png",
		},
	];
</script>

<Card title="Desayunos" />
<Menu_items {menu_items} />
