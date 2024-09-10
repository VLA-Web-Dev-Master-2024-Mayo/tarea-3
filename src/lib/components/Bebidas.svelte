<script lang="ts">
	type Menu = { title: string; page_link: string; img_src: string };

	const menu: Menu[] = [
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
