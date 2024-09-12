<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Menu_items, { type Menu_item as MMenu_item } from "$lib/components/Menu_item.svelte";
	let menu_items: MMenu_item[] = $state([]);

	menu_items = [
		{
			title: "McPapas Pequeñas",
			page_link: "",
			img_src: "/assets/paraacompanar/McPapas Pequeñas.png",
		},
		{
			title: "McPapas Medianas",
			page_link: "",
			img_src: "/assets/paraacompanar/McPapas Medianas.png",
		},
		{
			title: "McPapas Grandes",
			page_link: "",
			img_src: "/assets/paraacompanar/McPapas Grandes.png",
		},
		{
			title: "Papas Cheddar Bacon",
			page_link: "",
			img_src: "/assets/paraacompanar/Papas Cheddar Bacon.png",
		},
		{
			title: "Papas Kids (Cajita Feliz)",
			page_link: "",
			img_src: "/assets/paraacompanar/Papas Kids (Cajita Feliz).png",
		},
	];
</script>

<Card title="Para Acompanar" />
<Menu_items {menu_items} />
