<script lang="ts">
    import ProductCard from '$lib/componentes/ProductCard.svelte';
    import Nav from '$lib/componentes/Nav.svelte';
  
    let products = [
      { name: 'Coca-Cola', image: '/imagenes/bebidas/coca.png', description: 'Refrescate con nuestras deliciosas opciones de bebidas.', price: '$5.99' },
      { name: 'Coca-Cola Sin Azúcar', image: '/imagenes/bebidas/cocaSinAzu.png', description: 'Refrescate con nuestras deliciosas opciones de bebidas.', price: '$6.99' },
      { name: 'Ginger Ale', image: '/imagenes/bebidas/ginger.png', description: 'Un delicioso bebidas de dos piezas McCrispy.', price: '$5.99' },
      { name: 'Fanta Naranja', image: '/imagenes/bebidas/fuzTea.png', description: 'Refrescate con nuestras deliciosas opciones de bebidas.', price: '$6.99' },
      { name: 'Agua Embotellada', image: '/imagenes/bebidas/fantaNaranja.png', description: 'Refrescate con nuestras deliciosas opciones de bebidas.', price: '$5.99' },
      { name: 'Agua Embotellada', image: '/imagenes/bebidas/agua.png', description: 'Refrescate con nuestras deliciosas opciones de bebidas.', price: '$5.99' }
    ];
  </script>
  
  <Nav/>

  <h1 class="text-4xl p-6 font-bold mb-6 text-center">Bebidas</h1>
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
  