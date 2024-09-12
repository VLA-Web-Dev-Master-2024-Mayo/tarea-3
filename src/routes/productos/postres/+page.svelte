<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Menu_items, { type Menu_item as MMenu_item } from "$lib/components/Menu_item.svelte";
	let menu_items: MMenu_item[] = $state([]);

	menu_items = [
		{
			title: "Cono Vainillan",
			page_link: "",
			img_src: "/assets/postres/conovainilla.png",
		},
		{
			title: "Cono Chocolate",
			page_link: "",
			img_src: "/assets/postres/conochocolate.png",
		},
		{
			title: "Cono Combinado",
			page_link: "",
			img_src: "/assets/postres/conocombinado.png",
		},
		{
			title: "Sundae Caramelo",
			page_link: "",
			img_src: "/assets/postres/sundaecarmelo.png",
		},
		{
			title: "Sundae Chocolate",
			page_link: "",
			img_src: "/assets/postres/sundaechocolate.png",
		},
		{
			title: "Sundae Fresa",
			page_link: "",
			img_src: "/assets/postres/sundaefresa.png",
		},
		{
			title: "McFlurry Oreo",
			page_link: "",
			img_src: "/assets/postres/mcflurryoreo.png",
		},
		{
			title: "MacFlurry Kit Kat",
			page_link: "",
			img_src: "/assets/postres/mcflurrykitKat.png",
		},
		{
			title: "Pastel Manzana",
			page_link: "",
			img_src: "/assets/postres/pasteldemanzana.png",
		},
		{
			title: "Pastel Pina",
			page_link: "",
			img_src: "/assets/postres/pasteldepina.png",
		},
		{
			title: "Cheese Cake Pie",
			page_link: "",
			img_src: "/assets/postres/cheessecakepie.png",
		},
	];
</script>

<Card title="Postres" />
<Menu_items {menu_items} />
