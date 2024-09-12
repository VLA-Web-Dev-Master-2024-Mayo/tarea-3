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
	<ul class="flex flex-wrap justify-center gap-y-5">
		<!-- grid grid-cols-3 justify-center items-center" -->
		{#each menu_items as item}
			<li class="hover:border hover:border-yellow-500 group w-[250px]">
				<a
					href={item.page_link}
					class="flex flex-col items-center text-center group-hover:font-bold"
					><img src={item.img_src} alt="" class="h-auto" />{item.title}</a
				>
			</li>
		{/each}
	</ul>
</nav>
