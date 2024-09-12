<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Menu_items, { type Menu_item as MMenu_item } from "$lib/components/Menu_item.svelte";
	let menu_items: MMenu_item[] = $state([]);

	menu_items = [
		{
			title: "Frappe Capuccino",
			page_link: "",
			img_src: "/assets/mccafe/frappecapuccino.png",
		},
		{
			title: "Frappe Caramelo",
			page_link: "",
			img_src: "/assets/mccafe/frappecaramelo.png",
		},
		{
			title: "Frappe Chai",
			page_link: "",
			img_src: "/assets/mccafe/frappechai.png",
		},
		{
			title: "Frappe Chocomenta",
			page_link: "",
			img_src: "/assets/mccafe/frappechocomenta.png",
		},
		{
			title: "Frappe Mocca",
			page_link: "",
			img_src: "/assets/mccafe/frappemocca.png",
		},
		{
			title: "Frappe Oreo",
			page_link: "",
			img_src: "/assets/mccafe/frappeoreo.png",
		},
		{
			title: "Chai Tea",
			page_link: "",
			img_src: "/assets/mccafe/chaitea.png",
		},
		{
			title: "Chocolate",
			page_link: "",
			img_src: "/assets/mccafe/chocolate.png",
		},
		{
			title: "Capuccino Menta",
			page_link: "",
			img_src: "/assets/mccafe/capuccinomenta.png",
		},
		{
			title: "Capuccino Mocca",
			page_link: "",
			img_src: "/assets/mccafe/capuccinomocca.png",
		},
		{
			title: "Capuccino Vainilla Latte",
			page_link: "",
			img_src: "/assets/mccafe/capuccinovainillalatte.png",
		},
		{
			title: "Chocolate Freddo",
			page_link: "",
			img_src: "/assets/mccafe/chocolatefreddo.png",
		},
		{
			title: "Chocomenta",
			page_link: "",
			img_src: "/assets/mccafe/chocomenta.png",
		},
		{
			title: "Cafe con Leche",
			page_link: "",
			img_src: "/assets/mccafe/cafeconleche.png",
		},
	];
</script>

<Card title="McCafe" />
<Menu_items {menu_items} />
