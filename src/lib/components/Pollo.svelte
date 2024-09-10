<script lang="ts">
	type Menu = { title: string; page_link: string; img_src: string };

	const menu: Menu[] = [
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

<nav>
	<ul class="grid grid-cols-3 grid-rows-2 justify-center">
		{#each menu as item}
			<li>
				<a href={item.page_link} class="flex flex-col items-center"
					><img src={item.img_src} alt="" />{item.title}</a
				>
			</li>
		{/each}
	</ul>
</nav>
