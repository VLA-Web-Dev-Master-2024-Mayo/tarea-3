<script lang="ts">
	type Menu = { title: string; page_link: string; img_src: string };

	const menu: Menu[] = [
		{
			title: "McPapas Pequeñas",
			page_link: "",
			img_src: "/assets/paraacompanar/McPapas Pequeñas.png",
		},
		{
			title: "McPapas Medianas",
			page_link: "",
			img_src: "/assets/paraacompanar/McPapas Medianas.png",
		},
		{
			title: "McPapas Grandes",
			page_link: "",
			img_src: "/assets/paraacompanar/McPapas Grandes.png",
		},
		{
			title: "Papas Cheddar Bacon",
			page_link: "",
			img_src: "/assets/paraacompanar/Papas Cheddar Bacon.png",
		},
		{
			title: "Papas Kids (Cajita Feliz)",
			page_link: "",
			img_src: "/assets/paraacompanar/Papas Kids (Cajita Feliz).png",
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
