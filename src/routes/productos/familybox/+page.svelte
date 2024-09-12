<script lang="ts">
	import Card from "$lib/components/Card.svelte";
	import Menu_items, { type Menu_item as MMenu_item } from "$lib/components/Menu_item.svelte";
	let menu_items: MMenu_item[] = $state([]);

	menu_items = [
		{
			title: "Family Box",
			page_link: "",
			img_src: "/assets/familybox/familybox.png",
		},
	];
</script>

<Card title="Family Box" />
<Menu_items {menu_items} />
<div class="w-[450px] text-gray-700 text-sm text-center m-auto">
	<p>
		¡La Mejor opción para compartir y combinas! 6 opciones a elegir a tu gusto entre: BigMac, Cuarto
		de Libra, 2 Hamburguesas con Queso, 2 pz. De pollo McCrispy o 10 McNuggets acompañados de
		McPapas Medianas o poder pedir también Cajita Feliz ¡Max 2! Elegí tambien la opción con refresos
		de 21 onzas para disfrutar.
	</p>
</div>
