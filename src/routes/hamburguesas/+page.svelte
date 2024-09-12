<script lang="ts">
    import ProductCard from '$lib/componentes/ProductCard.svelte';
    import Nav from '$lib/componentes/Nav.svelte';
  
    let products = [
      { name: 'Crispy Chicken Classic', image: '/imagenes/hamburguesas/crispyChickenClassic.png', description: 'Crujiente, jugoso y tierno sándwich de filete de pechuga de pollo con un nuevo y suave pan de papa con mantequilla acompañado de crujientes pepinillos.', price: '$5.99' },
      { name: 'Crispy Chicken Deluxe', image: '/imagenes/hamburguesas/crispyChickenDeluxe.png', description: 'Delicioso sándwich con todo el sabor de la pechuga de pollo, pepinillos y un toque spicy en un irresistible pan de papa.', price: '$6.99' },
      { name: 'McPollo', image: '/imagenes/hamburguesas/mcPollo.png', description: 'Hamburguesa con pan con ajonjoli, mayonesa y lechuga picada.', price: '$5.99' },
      { name: 'Big Mac', image: '/imagenes/hamburguesas/bigMac.png', description: 'Una famosa hamburguesa de McDonald´s por sus ingredientes como lo son tres panes, lechuga fresca, cebolla y deliciosos pepinillos, un queso amarillo, su salsa especial a base de pepinillo para finalizar con sus dos tortas de carne 100% Res.', price: '$6.99' },
      { name: 'MacNifica', image: '/imagenes/hamburguesas/macNifica.png', description: 'Un delicioso pan de ajonjolí con mayonesa, salsa de tomate, mostaza, cebolla, lechuga fresca, tomate y nuestra jugosa torta de carne 100% Res.', price: '$5.99' },
      { name: 'Premium Bacon', image: '/imagenes/hamburguesas/premiumBacon.png', description: 'Un pan con ajonjolí, salsa de tomate, mostaza, una rica cebolla morada con deliciosos pepinillos, crujientes tiras de tocino y dos deliciosos quesos amarillos.', price: '$6.99' }
    ];
  </script>

  <Nav/>
  
  <h1 class="text-4xl p-6 font-bold mb-6 text-center">Hamburguesas</h1>
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
  