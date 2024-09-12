<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Menu_items, { type Menu_item as MMenu_item } from "$lib/components/Menu_item.svelte";
	let menu_items: MMenu_item[] = $state([]);

	menu_items = [
		{
			title: "Ensalda Jardinera",
			page_link: "",
			img_src: "/assets/ensaladas/ensaladajardinera.png",
		},
		{
			title: "Ensalda con Pechuga Crispy",
			page_link: "",
			img_src: "/assets/ensaladas/ensaladaconpechugacrispy.png",
		},
	];
</script>

<Card title="Ensaladas" />
<Menu_items {menu_items} />
