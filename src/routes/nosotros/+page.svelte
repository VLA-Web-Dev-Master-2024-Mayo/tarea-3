<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Menu_items, { type Menu_item as MMenu_item } from "$lib/components/Menu_item.svelte";
	let menu_items: MMenu_item[] = $state([]);

	menu_items = [
		{
			title: "Arcos Dorados",
			page_link: "",
			img_src: "/assets/nosotros/arcosdorados.png",
		},
		{
			title: "Trabaja con Nosotros",
			page_link: "",
			img_src: "/assets/nosotros/trabajaconnosotros.png",
		},
		{
			title: "Noticias",
			page_link: "",
			img_src: "/assets/nosotros/noticias.png",
		},
		{
			title: "Compromiso Social y Desarrolo Sustentable",
			page_link: "",
			img_src: "/assets/nosotros/compromisosocial.png",
		},
		{
			title: "Contacto",
			page_link: "",
			img_src: "/assets/nosotros/contacto.png",
		},
	];
</script>

<Card title="Nosotros" />
<Menu_items {menu_items} />
