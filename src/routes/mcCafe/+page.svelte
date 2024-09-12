<script lang="ts">
    import ProductCard from '$lib/componentes/ProductCard.svelte';
    import Nav from '$lib/componentes/Nav.svelte';
  
    let products = [
      { name: 'Frappé Capuccino', image: '/imagenes/mcCafe/frappeCapuccino.png', description: 'Frappé Capuccino', price: '$5.99' },
      { name: 'Frappé Caramelo', image: '/imagenes/mcCafe/frappeCaramelo.png', description: 'Frappé Caramelo', price: '$6.99' },
      { name: 'Frappé Chai', image: '/imagenes/mcCafe/frappeChai.png', description: 'Frappé Chai', price: '$5.99' },
      { name: 'Chocolate', image: '/imagenes/mcCafe/chocolate.png', description: 'Chocolate', price: '$5.99' },
      { name: 'Café con Leche', image: '/imagenes/mcCafe/cafeConLeche.png', description: 'Acompañá tu producto favorito con un inigualables bebidas calientes', price: '$6.99' },
      { name: 'Chocomenta', image: '/imagenes/mcCafe/chocomenta.png', description: 'Chocomenta', price: '$5.99' }
    ];
  </script>

  <Nav/>
  
  <h1 class="text-4xl p-6 font-bold mb-6 text-center">Postres</h1>
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
  