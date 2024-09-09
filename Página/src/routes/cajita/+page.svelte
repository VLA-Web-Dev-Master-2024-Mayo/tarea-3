<script>
    // components
	import Footer from "$lib/components/Footer.svelte";
    import Navbar from "$lib/components/Navbar.svelte";

    // Imágenes
    import Hamburgesa from "$lib/assets/CajitaFeliz/Hamburguesa.png";
    import McPapas from "$lib/assets/CajitaFeliz/McPapas.png";
    import McNuggets from "$lib/assets/CajitaFeliz/McNuggets.png";
    import JugoManzana from "$lib/assets/CajitaFeliz/JugoManzana.png";
    import YogurtFresa from "$lib/assets/CajitaFeliz/YogurtFresa.png";

</script>

<Navbar />
    
    <main class="flex-grow p-12">

            <h1 class="flex justify-center text-3xl font-medium pr-4">Cajita Feliz</h1>
            <br>
            <br>

            <!-- Primera columna -->

        <div class="flex-row flex items-center justify-center gap-48">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Hamburguesa" 
                        src={Hamburgesa}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Hamburgesa</div>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Mc Papas" 
                        src={McPapas}
                        class="flex justify-center"
                        height="100"
                        width="110"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Mc Papas</div>
            </div>

            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Mc Nuggets" 
                        src={McNuggets}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Mc Nuggets</div>
            </div>
        </div>

        <br>
        <br>

                    <!-- Segunda columna -->

        <div class="flex-row flex items-center justify-center gap-48 mx-2">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Jugo de Manzana" 
                        src={JugoManzana}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Jugo de Manzana</div>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-14 flex flex-col place-items-center">
                    <img alt="Yogurt de Fresa" 
                        src={YogurtFresa}
                        class="flex justify-center"
                        height="130"
                        width="130"
                    />
                    <br>
                        <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Yogurt de Fresa</div>
            </div>
        </div>

    </main>
    
    <Footer />