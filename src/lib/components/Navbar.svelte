<script lang="ts">
	type Menu = { title: String; page_link: string };

	const menu: Menu[] = [
		{ title: "Productos", page_link: "/productos" },
		{ title: "Restaurantes", page_link: "" },
		{ title: "En Familia", page_link: "/enfamilia" },
		{ title: "Nosotros", page_link: "/nosotros" },
		{ title: "McDelivery", page_link: "/mcdelivery" },
		{ title: "Cupones", page_link: "" },
	];
</script>

<nav class="bg-#ffffff shadow-lg w-full flex justify-center gap-1">
	<img src="/assets/mcdonalds-logo-footer-bg-white.png" alt="logo" class="h-[140px]" />
	<ul class="flex justify-center items-end h-32 gap-5 font-speedee font-normal">
		{#each menu as item}
			<li class="hover:border-b-4 hover:border-yellow-500 h-10">
				<a href={item.page_link} class="p-4">{item.title}</a>
			</li>
		{/each}
	</ul>
</nav>
