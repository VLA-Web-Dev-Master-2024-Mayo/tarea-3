<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Menu_items, { type Menu_item as MMenu_item } from "$lib/components/Menu_item.svelte";
	let menu_items: MMenu_item[] = $state([]);

	menu_items = [
		{
			title: "Coca-Cola",
			page_link: "",
			img_src: "/assets/bebidas/Coca-Cola.png",
		},
		{
			title: "Coca-Cola Sin Azucar",
			page_link: "",
			img_src: "/assets/bebidas/Coca-Cola-sinazucar.png",
		},
		{
			title: "Ginger Ale",
			page_link: "",
			img_src: "/assets/bebidas/Gingerale.png",
		},
		{
			title: "Fanta Naranja",
			page_link: "",
			img_src: "/assets/bebidas/Fantanaranja.png",
		},
		{
			title: "Fuze Tea",
			page_link: "",
			img_src: "/assets/bebidas/Fuzetea.png",
		},
		{
			title: "Fuze Tea Cero",
			page_link: "",
			img_src: "/assets/bebidas/Fuzeteacero.png",
		},
		{
			title: "Cafe Americano",
			page_link: "",
			img_src: "/assets/bebidas/Cafeamericano.png",
		},
		{
			title: "Capuccino",
			page_link: "",
			img_src: "/assets/bebidas/Capuccino.png",
		},
		{
			title: "Late",
			page_link: "",
			img_src: "/assets/bebidas/Late.png",
		},
		{
			title: "Jugo de Naranja",
			page_link: "",
			img_src: "/assets/bebidas/Jugonaranja.png",
		},
		{
			title: "Agua Embotellada",
			page_link: "",
			img_src: "/assets/bebidas/Aguaembotellada.png",
		},
		{
			title: "Nectar de Manzana",
			page_link: "",
			img_src: "/assets/bebidas/Nectardemanzana.png",
		},
		{
			title: "Te",
			page_link: "",
			img_src: "/assets/bebidas/Te.png",
		},
	];
</script>

<Card title="Bebidas" />
<Menu_items {menu_items} />
