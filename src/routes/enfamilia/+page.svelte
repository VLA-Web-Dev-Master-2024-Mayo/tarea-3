<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Menu_items, { type Menu_item as MMenu_item } from "$lib/components/Menu_item.svelte";
	let menu_items: MMenu_item[] = $state([]);

	menu_items = [
		{
			title: "Cajita Feliz",
			page_link: "",
			img_src: "/assets/enfamilia/cajitafeliz.png",
		},
		{
			title: "Cajita Feliz Juguete",
			page_link: "",
			img_src: "/assets/enfamilia/cajitafelizjuguete.png",
		},
		{
			title: "Family Box",
			page_link: "",
			img_src: "/assets/enfamilia/familybox.png",
		},
		{
			title: "Con Las Familias",
			page_link: "",
			img_src: "/assets/enfamilia/compromisoconlasfamilias.png",
		},
		{
			title: "McDonald's Land'",
			page_link: "",
			img_src: "/assets/enfamilia/mcdonaldsland.png",
		},
	];
</script>

<Card title="En Familia" />
<Menu_items {menu_items} />
