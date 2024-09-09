<script>
    // components
	import Footer from "$lib/components/Footer.svelte";
    import Navbar from "$lib/components/Navbar.svelte";

    // Imágenes
    import CafeLeche from "$lib/assets/McCafes/CafeConLeche.png";
    import FrappeCapuccino from "$lib/assets/McCafes/FrappeCapuccino.png";
    import FrappeCaramelo from "$lib/assets/McCafes/FrappeCaramelo.png";
    import FrappeChai from "$lib/assets/McCafes/FrappeChai.png";
    import FrappeChocomenta from "$lib/assets/McCafes/FrappeChocomenta.png";

</script>

<Navbar />
    
    <main class="flex-grow p-12">

            <h1 class="flex justify-center text-3xl font-medium pr-4">Mc Cafés</h1>
            <br>
            <br>

            <!-- Primera columna -->

        <div class="flex-row flex items-center justify-center gap-48">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-20 px-16 flex flex-col place-items-center">
                    <img alt="Café con Leche" 
                        src={CafeLeche}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Café con Leche</div>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Frappe Caramelo" 
                        src={FrappeCaramelo}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Frappe Caramelo</div>
            </div>

            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Frappe Chai" 
                        src={FrappeChai}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Frappe Chai</div>
            </div>
        </div>

        <br>
        <br>

                    <!-- Segunda columna -->

        <div class="flex-row flex items-center justify-center gap-48 mx-2">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-20 px-16 flex flex-col place-items-center">
                    <img alt="Frappe Chocomenta" 
                        src={FrappeChocomenta}
                        class="flex justify-center"
                        height="110"
                        width="110"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Frappe Chocomenta</div>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-16 flex flex-col place-items-center">
                    <img alt="Frappe Capuccino" 
                        src={FrappeCapuccino}
                        class="flex justify-center"
                        height="110"
                        width="110"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Frappe Capuccino</div>
            </div>
        </div>

    </main>
    
    <Footer />