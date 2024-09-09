<script>
    // components
	import Footer from "$lib/components/Footer.svelte";
    import Navbar from "$lib/components/Navbar.svelte";

    // Imágenes
    import ConoCombinado from "$lib/assets/Helados/ConoCombinado.png";
    import Kitkat from "$lib/assets/Helados/McFlurryKitKat.png";
    import Oreo from "$lib/assets/Helados/McFlurryOreo.png";
    import ShakeCaramelo from "$lib/assets/Helados/McShakeCaramelo.png";
    import ShakeMaracuya from "$lib/assets/Helados/McShakeMaracuya.png";
    import SundaeFresa from "$lib/assets/Helados/SundaeFresa.png";

</script>

<Navbar />
    
    <main class="flex-grow p-12 justify-center">

            <h1 class="flex justify-center text-3xl font-medium pr-4">Helados</h1>
            <br>
            <br>

            <!-- Primera columna -->

        <div class="flex-row flex items-center justify-center gap-48 mx-12">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 px-8 flex flex-col place-items-center">
                    <img alt="Cono Combinado Vainilla y Chocolate" 
                        src={ConoCombinado}
                        class="flex justify-center"
                        height="110"
                        width="110"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Cono Vainilla y Chocolate</div>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-14 px-18 flex flex-col place-items-center">
                    <img alt="Mc Flurry KitKat" 
                        src={Kitkat}
                        class="flex justify-center"
                        height="140"
                        width="140"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Mc Flurry KitKat</div>
            </div>

            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 px-18 flex flex-col place-items-center">
                    <img alt="Mc Flurry Oreo" 
                        src={Oreo}
                        class="flex justify-center"
                        height="140"
                        width="140"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Mc Flurry Oreo</div>
            </div>
        </div>

        <br>
        <br>

                    <!-- Segunda columna -->

        <div class="flex-row flex items-center justify-center gap-48 mx-2">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 px-14 ml-6 flex flex-col place-items-center">
                    <img alt="Mc Shake Caramelo" 
                        src={ShakeCaramelo}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Mc Shake Caramelo</div>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-14 px-12 flex flex-col place-items-center">
                    <img alt="Mc Shake Maracuya" 
                        src={ShakeMaracuya}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Mc Shake Maracuya</div>
            </div>

            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 px-14 mr-8 flex flex-col place-items-center">
                    <img alt="Sundae Fresa" 
                        src={SundaeFresa}
                        class="flex justify-center"
                        height="130"
                        width="130"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Sundae Fresa</div>
            </div>
        </div>

    </main>

    <Footer />