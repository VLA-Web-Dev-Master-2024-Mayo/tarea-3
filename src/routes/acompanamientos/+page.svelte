<script lang="ts">
    import ProductCard from '$lib/componentes/ProductCard.svelte';
    import Nav from '$lib/componentes/Nav.svelte';
  
    let products = [
      { name: 'McPapas Pequeñas', image: '/imagenes/acompanamientos/mcPapasPeque.png', description: 'Calientes, crujientes y deliciosas. Disfrutá de nuestras papas mundialmente famosas, desde la primera hasta la última.', price: '$5.99' },
      { name: 'McPapas Medianas', image: '/imagenes/acompanamientos/mcPapasMedi.png', description: 'Calientes, crujientes y deliciosas. Disfrutá de nuestras papas mundialmente famosas, desde la primera hasta la última.', price: '$6.99' },
      { name: 'McPapas Grandes', image: '/imagenes/acompanamientos/mcPapasGran.png', description: 'Calientes, crujientes y deliciosas. Disfrutá de nuestras papas mundialmente famosas, desde la primera hasta la última.', price: '$5.99' },
      { name: 'Papas Cheddar Bacon', image: '/imagenes/acompanamientos/papasCheddar.png', description: 'Calientes, deliciosas, crujientes y ademas agregale bacon con queso cheddaar fundido. Disfrutá de nuestras papas mundialmente famosas, desde la primera hasta la última.', price: '$6.99' },
      { name: 'Papas Kids (Cajita Feliz)', image: '/imagenes/acompanamientos/papasKids.png', description: 'Papas, aceite de girasol, dextrosa y estabilizante: ácido pirofosfato de sodio (ISN 450 i), sal.', price: '$5.99' }
    ];
  </script>

  <Nav/>

  <h1 class="text-4xl p-6 font-bold mb-6 text-center">Para Acompañar</h1>
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
  