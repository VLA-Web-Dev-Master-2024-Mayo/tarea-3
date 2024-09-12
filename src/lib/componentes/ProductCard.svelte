<script lang="ts">
 
  interface Props {
    name: string;
    description: string;
    price: string;
    image: string;
  }

  const { name, description, price, image }: Props = $props();
</script>

  <div class="max-w-xs rounded overflow-hidden shadow-lg bg-white transition transform hover:scale-105 hover:shadow-2xl">
    <div class="w-full h-32 flex items-center justify-center overflow-hidden">
      <img class="object-contain w-full h-full" src={image} alt={name} />
    </div>
    <div class="p-4">
      <h2 class="font-bold text- mb-3">{name}</h2> <!-- Tamaño del texto reducido -->
      <p class="text-gray-700 text-md mb-3">{description}</p> <!-- Tamaño del texto reducido -->
      <p class="text-yellow-600 text-sm font-semibold">{price}</p> <!-- Tamaño del texto reducido -->
    </div>
  </div>
