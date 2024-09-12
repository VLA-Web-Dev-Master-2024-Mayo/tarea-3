<script lang="ts">
    import ProductCard from '$lib/componentes/ProductCard.svelte';
    import Nav from '$lib/componentes/Nav.svelte';
  
    let products = [
      { name: 'McMuffin', image: '/imagenes/desayunos/mcMuffin.png', description: 'McDonald´s tiene un delicioso y clasico desayuno para iniciar el día. Disfrutá un delicioso pan muffin calientito con huevo, un rico jamón canadiense y queso amarillo.', price: '$5.99' },
      { name: 'Huevos Revueltos con Salchicha y Muffin', image: '/imagenes/desayunos/huevosRevueltos.png', description: 'Disfrutá de un delicioso y calientito pan muffin con exquisita salchicha y queso tipo americano. Pedilo en McCombo con papa rallada y un nutritivo jugo de naranja o un aromático café premium.', price: '$6.99' },
      { name: 'McPinto Deluxe', image: '/imagenes/desayunos/mcPintoDeluxe.png', description: 'Nuestro tradicional McPinto. Vení a disfrutar el sabor de nuestro McPinto acompañado de huevos revueltos, cremosa natilla, dorados platanos maduros, salchicha y unas tortillas calientitas.', price: '$5.99' },
      { name: 'McPinto con Huevo', image: '/imagenes/desayunos/mcPintoHuevo.png', description: 'Nuestro tradicional McPinto. Vení a disfrutar el sabor de nuestro McPinto acompañado de huevos revueltos, cremosa natilla y unas tortillas calientitas.', price: '$6.99' },
      { name: 'Pancake', image: '/imagenes/desayunos/pancake.png', description: 'Deliciosos Pan cakes cremosos con la perfecta combinación de mapple para inicar la mañana.', price: '$5.99' },
      { name: 'Empanada de Carne', image: '/imagenes/desayunos/empanadaCarne.png', description: 'Empanada de Carne', price: '$5.99' }
    ];
  </script>
  
  <Nav/>

  <h1 class="text-4xl p-6 font-bold mb-6 text-center">Desayunos</h1>
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
  