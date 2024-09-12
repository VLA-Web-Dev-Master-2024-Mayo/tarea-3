<script lang="ts">
	type Menu = { title: string; page_link: string; img_src: string };

	const menu: Menu[] = [
		{
			title: "Hamburguesas",
			page_link: "/productos/hamburguesas",
			img_src: "/assets/menuprincipal/hamburguesa.png",
		},
		{
			title: "Pollo",
			page_link: "/productos/Pollo",
			img_src: "/assets/menuprincipal/pollo.png",
		},
		{
			title: "Para Acompanar",
			page_link: "/productos/paraacompanar",
			img_src: "/assets/menuprincipal/paraacompanar.png",
		},
		{
			title: "Bebidas",
			page_link: "/productos/bebidas",
			img_src: "/assets/menuprincipal/bebidas.png",
		},
		{
			title: "Postres",
			page_link: "/productos/postres",
			img_src: "/assets/menuprincipal/postres.png",
		},
		{
			title: "cajitafeliz",
			page_link: "/productos/cajitafeliz",
			img_src: "/assets/menuprincipal/cajitafeliz.png",
		},
		{
			title: "cajitafelizdesayuno",
			page_link: "/productos/cajitafelizdesayuno",
			img_src: "/assets/menuprincipal/cajitafelizdesayuno.png",
		},
		{
			title: "familybox",
			page_link: "/productos/familybox",
			img_src: "/assets/menuprincipal/familybox.png",
		},
		{
			title: "Ensaladas",
			page_link: "/productos/ensaladas",
			img_src: "/assets/menuprincipal/salads.png",
		},
		{
			title: "Desayunos",
			page_link: "/productos/desayunos",
			img_src: "/assets/menuprincipal/desayunos.png",
		},
		{
			title: "McCafe",
			page_link: "/productos/mccafe",
			img_src: "/assets/menuprincipal/maccafe.png",
		},
	];
</script>

<nav class="relative ml-10 mr-10 z-[500] mt-[50px]">
	<ul class="grid grid-cols-4 gap-y-5 border p-5">
		{#each menu as item}
			<li class="hover:border-b-2 hover:border-yellow-500 group">
				<a
					href={item.page_link}
					class="flex flex-col items-center text-[18px] group-hover:font-bold"
					><img
						src={item.img_src}
						alt=""
						class="ml-[6px] mr-[12px] h-auto w-[75px]"
					/>{item.title}</a
				>
			</li>
		{/each}
	</ul>
</nav>
