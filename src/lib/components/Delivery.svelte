<script lang="ts" module>
	export type Menu_item = { title: string; page_link: string; img_src: string };
</script>

<script lang="ts">
	type Props = { menu_items: Menu_item[] };
	const { menu_items }: Props = $props();

	/* const defaultMenus = menus.map((menu) => ({
		title: menu.title ?? "Título por defecto",
		page_link: menu.page_link ?? "/",
		img_src: menu.img_src ?? "/images/default.png",
	})); */
</script>

<nav class="relative ml-10 mr-10 mt-[50px]">
	<ul class="flex flex-wrap justify-center gap-x-10">
		<!-- grid grid-cols-3 justify-center items-center" -->
		{#each menu_items as item}
			<li class="border border-gray-300 hover:border hover:border-yellow-500 group w-[250px]">
				<div class="flex flex-col justify-center items-center">
					<a
						href={item.page_link}
						class="flex flex-col items-center text-center group-hover:font-bold"
						><img src={item.img_src} alt="" class="h-auto" />{item.title}</a
					>
					<button class="p-2 rounded w-[125px] bg-yellow-500 border hover:bg-yellow-700 mb-5"
						>Ordena aqui</button
					>
				</div>
			</li>
		{/each}
	</ul>
</nav>
