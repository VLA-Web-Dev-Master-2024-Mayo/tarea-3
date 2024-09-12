<script lang="ts">

  import Nav from '$lib/componentes/Nav.svelte';

  let categories = [
    { name: "Hamburguesas", image: "/imagenes/menu/hamburguesas.png", link: "/hamburguesas" },
    { name: "Pollo", image: "/imagenes/menu/pollo.png", link: "/pollo" },
    { name: "Acompañamientos", image: "/imagenes/menu/acompanamientos.png", link: "/acompanamientos" },
    { name: "Bebidas", image: "/imagenes/menu/bebidas.png", link: "/bebidas" },
    { name: "Postres", image: "/imagenes/menu/postres.png", link: "/postres" },
   
    { name: "Ensaladas", image: "/imagenes/menu/ensaladas.png", link: "/ensaladas" },
    { name: "Desayunos", image: "/imagenes/menu/desayunos.png", link: "/desayunos" },
    { name: "McCafé", image: "/imagenes/menu/mcCafe.png", link: "/mcCafe" },
  ];
</script>

 <Nav/>

<h1 class="text-4xl p-6 font-bold mb-6 text-center">Nuestros productos</h1>

<div class="border border-gray-300 p-6 rounded-lg max-w-screen-lg mx-auto my-8">
  <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
    {#each categories as category}
      <a href={category.link} class="block text-center">
        <div class="p-4 rounded-lg hover:shadow-lg transition flex flex-col items-center justify-center">
          <div class="w-20 h-20">
            <img src={category.image} alt={category.name} class="w-full h-full object-cover rounded" />
          </div>
          <h2 class="text-lg">{category.name}</h2>
        </div>
      </a>
    {/each}
  </div>
</div>
