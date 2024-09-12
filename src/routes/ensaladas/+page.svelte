<script lang="ts">
    import ProductCard from '$lib/componentes/ProductCard.svelte';
    import Nav from '$lib/componentes/Nav.svelte';
  
    let products = [
      { name: 'Ensalada Jardinera', image: '/imagenes/ensaladas/ensaladaJardi.png', description: 'Disfruta de una rica ensalada verde, con tomate, maíz dulce, queso emmental junto con su aderezo.', price: '$5.99' },
      { name: 'Ensalada con Pechuga Crispy', image: '/imagenes/ensaladas/ensaladaPechugaCrispy.png', description: 'Disfruta de una rica ensalada verde, con tomate, maíz dulce, queso emmental, torta de pollo crispy, todo esto junto a su aderezo.', price: '$6.99' },
    ];
  </script>
  
  <Nav/>

  <h1 class="text-4xl p-6 font-bold mb-6 text-center">Ensaladas</h1>
  <div class=" p-6 rounded-lg max-w-screen-lg mx-auto my-8">
  <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
    {#each products as product}
      <ProductCard
        name={product.name}
        description={product.description}
        price={product.price}
        image={product.image}
      />
    {/each}
  </div>
</div>
  