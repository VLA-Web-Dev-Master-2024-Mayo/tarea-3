<script>
    // components
	import Footer from "$lib/components/Footer.svelte";
    import Navbar from "$lib/components/Navbar.svelte";

    // Imágenes
    import Coke from "$lib/assets/Bebidas/Coke.png";
    import Fanta from "$lib/assets/Bebidas/Fanta.png";
    import FuzeTea from "$lib/assets/Bebidas/FuzeTea.png";
    import Ginger from "$lib/assets/Bebidas/Ginger.png";
    import JugoNaranja from "$lib/assets/Bebidas/JugoNaranja.png";

</script>

<Navbar />
    
    <main class="flex-grow p-12">

            <h1 class="flex justify-center text-3xl font-medium pr-4">Bebidas</h1>
            <br>
            <br>

            <!-- Primera columna -->

        <div class="flex-row flex items-center justify-center gap-48">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Coca-cola" 
                        src={Coke}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Coca-Cola</div>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Fanta" 
                        src={Fanta}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Fanta</div>
            </div>

            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Fuze tea" 
                        src={FuzeTea}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Fuze Tea</div>
            </div>
        </div>

        <br>
        <br>

                    <!-- Segunda columna -->

        <div class="flex-row flex items-center justify-center gap-48 mx-2">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Ginger ale" 
                        src={Ginger}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Ginger Ale</div>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Jugo de Naranja" 
                        src={JugoNaranja}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Jugo de Naranja</div>
            </div>
        </div>

    </main>
    
    <Footer />