<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Menu_items, { type Menu_item as MMenu_item } from "$lib/components/Menu_item.svelte";
	let menu_items: MMenu_item[] = $state([]);

	menu_items = [
		{
			title: "McNuggets 4 pz",
			page_link: "",
			img_src: "/assets/Pollo/McNuggets4pz.png",
		},
		{
			title: "McNuggets 10 pz",
			page_link: "",
			img_src: "/assets/Pollo/McNuggets10pz.png",
		},
		{
			title: "2 pz. Pollo McCrispy",
			page_link: "",
			img_src: "/assets/Pollo/2pzPolloMcCrispy.png",
		},
		{
			title: "Pollo McCrispy",
			page_link: "",
			img_src: "/assets/Pollo/3pzPolloMcCrispy.png",
		},
		{
			title: "1 pz. Pollo McCrispy",
			page_link: "",
			img_src: "/assets/Pollo/1pzPolloMcCrispy.png",
		},
	];
</script>

<Card title="Pollo" />
<Menu_items {menu_items} />
