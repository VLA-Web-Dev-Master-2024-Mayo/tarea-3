<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Delivery, { type Menu_item as MMenu_item } from "$lib/components/Delivery.svelte";
	let menu_items: MMenu_item[] = $state([]);

	menu_items = [
		{
			title: "",
			page_link: "",
			img_src: "/assets/mcdelivery/didi.png",
		},
		{
			title: "",
			page_link: "",
			img_src: "/assets/mcdelivery/pedidosya.png",
		},
		{
			title: "",
			page_link: "",
			img_src: "/assets/mcdelivery/ubereats.png",
		},
	];
</script>

<Card title="McDelivery" />
<img src="/assets/mcdelivery/mcdelivery.png" alt="" class="h-[350px]" />
<Delivery {menu_items} />
