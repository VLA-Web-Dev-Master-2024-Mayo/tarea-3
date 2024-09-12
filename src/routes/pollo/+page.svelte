<script lang="ts">
    import ProductCard from '$lib/componentes/ProductCard.svelte';
    import Nav from '$lib/componentes/Nav.svelte';
  
    let products = [
      { name: 'McNuggets 4 pz.', image: '/imagenes/pollo/mcNuggets4.png', description: 'Disfrutá 4 unidades de McNuggets con su salsa favorita.', price: '$5.99' },
      { name: 'McNuggets 4 pz.', image: '/imagenes/pollo/mcNuggets10.png', description: 'Disfrutá 10 unidades de McNuggets con su salsa favorita.', price: '$6.99' },
      { name: 'Pollo McCrispy 2 pz.', image: '/imagenes/pollo/polloMcCrispy2.png', description: 'Un delicioso pollo de dos piezas McCrispy.', price: '$5.99' },
      { name: 'Pollo McCrispy 3 pz.', image: '/imagenes/pollo/polloMcCrispy3.png', description: 'Un delicioso pollo de tres piezas McCrispy.', price: '$6.99' },
      { name: 'Pollo McCrispy 1 pz', image: '/imagenes/pollo/polloMcCrispy1.png', description: 'Una deliciosa pieza de pollo McCrispy.', price: '$5.99' },
      
    ];
  </script>
  
  <Nav/>

  <h1 class="text-4xl p-6 font-bold mb-6 text-center">Pollo</h1>
  <div class="p-6 rounded-lg max-w-screen-lg mx-auto my-8">
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
  