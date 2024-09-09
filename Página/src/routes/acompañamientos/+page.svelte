<script>
    // components
	import Footer from "$lib/components/Footer.svelte";
    import Navbar from "$lib/components/Navbar.svelte";

    // Imágenes
    import PapasPequeñas from "$lib/assets/Acompañamientos/McPapasPequeñas.png";
    import PapasMedianas from "$lib/assets/Acompañamientos/McPapasMedianas.png";
    import PapasGrandes from "$lib/assets/Acompañamientos/McPapasGrandes.png";
    import PapasCheddar from "$lib/assets/Acompañamientos/PapasCheddarBacon.png";


</script>

<Navbar />
    
    <main class="flex-grow p-12">

            <h1 class="flex justify-center text-3xl font-medium pr-4">Acompañamientos</h1>
            <br>
            <br>

            <!-- Primera columna -->

        <div class="flex-row flex items-center justify-center gap-48">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Papas Pequeñas" 
                        src={PapasPequeñas}
                        class="flex justify-center"
                        height="150"
                        width="140"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Mc Papas Pequeñas</div>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Papas Medianas" 
                        src={PapasMedianas}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Mc Papas Medianas</div>
            </div>

            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Papas Grandes" 
                        src={PapasGrandes}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Mc Papas Grandes</div>
            </div>
        </div>

        <br>
        <br>

                    <!-- Segunda columna -->

        <div class="flex-row flex items-center justify-center gap-48 mx-2">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Papas Cheddar con Bacon" 
                        src={PapasCheddar}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Papas Cheddar con Bacon</div>
            </div>
    </main>

    <Footer />