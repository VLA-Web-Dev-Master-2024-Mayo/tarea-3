<script>
    // components
	import Footer from "$lib/components/Footer.svelte";
    import Navbar from "$lib/components/Navbar.svelte";

    // Imágenes
    import EggMcMuffin from "$lib/assets/Desayunos/EggMcMuffin.png";
    import McMuffin from "$lib/assets/Desayunos/McMuffin.png";
    import McPinto from "$lib/assets/Desayunos/McPinto.png";
    import Pancakes from "$lib/assets/Desayunos/Pancakes.png";


</script>

<Navbar />
    
    <main class="flex-grow p-12">

            <h1 class="flex justify-center text-3xl font-medium pr-6">Desayunos</h1>
            <br>
            <br>

            <!-- Primera columna -->

        <div class="flex-row flex items-center justify-center gap-48">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 px-16 flex flex-col place-items-center">
                    <img alt="Egg Mc Muffin" 
                        src={EggMcMuffin}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Egg Mc Muffin</div>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Mc Muffin" 
                        src={McMuffin}
                        class="flex justify-center"
                        height="140"
                        width="140"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Mc Muffin</div>
            </div>

            <div class="border-2 border-yellow-200 bg-white rounded-md p-16 px-8 flex flex-col place-items-center">
                    <img alt="Mc Pinto" 
                        src={McPinto}
                        class="flex justify-center"
                        height="120"
                        width="200"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Mc Pinto</div>
            </div>
        </div>

        <br>
        <br>

                    <!-- Segunda columna -->

        <div class="flex-row flex items-center justify-center gap-48 mx-2">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-16 px-16 mr-3 flex flex-col place-items-center">
                    <img alt="Pancakes" 
                        src={Pancakes}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Pancakes</div>
            </div>
    </main>

    <Footer />