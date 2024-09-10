<script lang="ts">
	type Menu = { title: string; page_link: string; img_src: string };

	const menu: Menu[] = [
		{
			title: "Hamburguesas",
			page_link: "/src/routes/productos/hamburguesas/+page.svelte",
			img_src: "/assets/menuprincipal/hamburguesa.png",
		},
		{
			title: "Pollo",
			page_link: "/src/routes/productos/Pollo/+page.svelte",
			img_src: "/assets/menuprincipal/pollo.png",
		},
		{
			title: "Bebidas",
			page_link: "/src/routes/productos/bebidas/+page.svelte",
			img_src: "/assets/menuprincipal/bebidas.png",
		},
		{
			title: "Postres",
			page_link: "/src/routes/productos/postres/+page.svelte",
			img_src: "/assets/menuprincipal/postres.png",
		},
		{
			title: "cajitafeliz",
			page_link: "/src/routes/productos/cajitafeliz/+page.svelte",
			img_src: "/assets/menuprincipal/cajitafeliz.png",
		},
		{
			title: "cajitafelizdesayuno",
			page_link: "/src/routes/productos/cajitafelizdesayuno/+page.svelte",
			img_src: "/assets/menuprincipal/cajitafelizdesayuno.png",
		},
		{
			title: "familybox",
			page_link: "/src/routes/productos/familybox/+page.svelte",
			img_src: "/assets/menuprincipal/familybox.png",
		},
		{
			title: "Ensaladas",
			page_link: "/src/routes/productos/ensaladas/+page.svelte",
			img_src: "/assets/menuprincipal/salads.png",
		},
		{
			title: "Desayunos",
			page_link: "/src/routes/productos/desayunos/+page.svelte",
			img_src: "/assets/menuprincipal/desayunos.png",
		},
		{
			title: "McCafe",
			page_link: "/src/routes/productos/mccafe/+page.svelte",
			img_src: "/assets/menuprincipal/maccafe.png",
		},
	];
</script>

<nav class="relative ml-28 z-[500] mt-[300px]">
	<ul class="flex flex-col border w-[300px]">
		{#each menu as item}
			<li class="hover:border-l-2 hover:border-yellow-500 group">
				<a
					href={item.page_link}
					class="flex items-center p-[0px_12px_0px_6px] text-[18px] h-[80px] group-hover:font-bold"
					><img
						src={item.img_src}
						alt=""
						class="ml-[6px] mr-[12px] h-auto w-[75px] max-h-full"
					/>{item.title}</a
				>
			</li>
		{/each}
	</ul>
</nav>
