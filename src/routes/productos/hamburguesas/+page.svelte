<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Menu_items, { type Menu_item as MMenu_item } from "$lib/components/Menu_item.svelte";
	let menu_items: MMenu_item[] = $state([]);

	menu_items = [
		{
			title: "Crispy Chicken Classic",
			page_link: "",
			img_src: "/assets/hamburguesas/crispychickenclassic.png",
		},
		{
			title: "Crispy Chicken Spicy",
			page_link: "",
			img_src: "/assets/hamburguesas/crispychickenspicy.png",
		},
		{
			title: "Crispy Chicken Deluxe",
			page_link: "",
			img_src: "/assets/hamburguesas/crispychickendeluxe.png",
		},
		{
			title: "Mac Pollo",
			page_link: "",
			img_src: "/assets/hamburguesas/macpollo.png",
		},
		{
			title: "Club House Pollo Crispy",
			page_link: "",
			img_src: "/assets/hamburguesas/clubhousepollocrispy.png",
		},
		{
			title: "Hongos Deluxe Pollo Crispy",
			page_link: "",
			img_src: "/assets/hamburguesas/hongosdeluxepollocrispy.png",
		},
	];
</script>

<Card title="Hamburguesas" />
<Menu_items {menu_items} />
