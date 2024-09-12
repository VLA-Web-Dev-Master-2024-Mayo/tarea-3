<script lang="ts">
    import ProductCard from '$lib/componentes/ProductCard.svelte';
    import Nav from '$lib/componentes/Nav.svelte';
  
    let products = [
      { name: 'Cono de Vainilla', image: '/imagenes/postres/conoVainilla.png', description: 'Delicioso Cono Crujiente acompañado de Cremoso helado de Vainilla', price: '$5.99' },
      { name: 'Sundae Caramello', image: '/imagenes/postres/sundaeCaramello.png', description: 'Helado de vainilla acompañado con topping de Caramelo', price: '$6.99' },
      { name: 'McFlurry Oreo', image: '/imagenes/postres/mcFlurryOreo.png', description: 'Delicioso y exclusivo helado de McDonald´s acompañado con el topping de su preferencia y combinado con oreo. El Favorito de muchos.', price: '$5.99' },
      { name: 'McShake Fresa', image: '/imagenes/postres/mcShakeFresa.png', description: 'Exquisito McShake a base de leche, helado y combinación de tu sabor favorito a Fresa', price: '$6.99' },
      { name: 'Pastel de Manzana', image: '/imagenes/postres/pastelManzana.png', description: 'Crujiente y calientito pastel de Manzana para disfrutar', price: '$5.99' },
      { name: 'Coffe Shake', image: '/imagenes/postres/coffeShake.png', description: 'Helado de Vainilla y Café Ameicano', price: '$5.99' }
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
  