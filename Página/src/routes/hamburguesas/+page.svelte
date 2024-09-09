<script>
    // components
	import Footer from "$lib/components/Footer.svelte";
    import Navbar from "$lib/components/Navbar.svelte";

    // Imágenes
    import ClubHouse from "$lib/assets/Hamburguesas/ClubHousePolloCrispy.png";
    import CrispySpicy from "$lib/assets/Hamburguesas/CrispyChickenSpicy.png";
    import CuartoLibra from "$lib/assets/Hamburguesas/CuartoDeLibraConQueso.png";
    import BigMac from "$lib/assets/Hamburguesas/BigMac.png";
    import McPollo from "$lib/assets/Hamburguesas/McPollo.png";
    import TripleBacon from "$lib/assets/Hamburguesas/TripleConBacon.png";

</script>

<Navbar />
    
    <main class="flex-grow p-12">

            <h1 class="flex justify-center text-3xl font-medium pr-4">Hamburgesas</h1>
            <br>
            <br>

            <!-- Primera columna -->

        <div class="flex-row flex items-center justify-center gap-48">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-16 flex flex-col place-items-center">
                    <img alt="Club House Pollo Crispy" 
                        src={ClubHouse}
                        class="flex justify-center"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Club House Pollo Crispy</div>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-16 flex flex-col place-items-center">
                    <img alt="Crispy Chicken Spicy" 
                        src={CrispySpicy}
                        class="flex justify-center"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Crispy Chicken Spicy</div>
            </div>

            <div class="border-2 border-yellow-200 bg-white rounded-md p-16 flex flex-col place-items-center">
                    <img alt="Cuarto De Libra Con Queso" 
                        src={CuartoLibra}
                        class="flex justify-center"
                        height="180"
                        width="180"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Cuarto De Libra Con Queso</div>
            </div>
        </div>

        <br>
        <br>

                    <!-- Segunda columna -->

        <div class="flex-row flex items-center justify-center gap-48 mx-2">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-16 px-16 flex flex-col place-items-center">
                    <img alt="Club House Pollo Crispy" 
                        src={BigMac}
                        class="flex justify-center"
                        height="180"
                        width="180"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Big Mac</div>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-16 flex flex-col place-items-center">
                    <img alt="Crispy Chicken Spicy" 
                        src={McPollo}
                        class="flex justify-center"
                        height="170"
                        width="190"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Mc Pollo</div>
            </div>

            <div class="border-2 border-yellow-200 bg-white rounded-md p-16 flex flex-col place-items-center">
                    <img alt="Cuarto De Libra Con Queso" 
                        src={TripleBacon}
                        class="flex justify-center"
                        height="180"
                        width="200"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Triple con Bacon</div>
            </div>
        </div>

    </main>

    <Footer />