<script>
    // components
	import Footer from "$lib/components/Footer.svelte";
    import Navbar from "$lib/components/Navbar.svelte";

    // Imágenes
    import FamilyBox from "$lib/assets/FamilyBox/FamilyBox.png";


</script>

<div class="flex flex-col min-h-screen max-w-full justify-center">
    <Navbar />

    <main class="flex-grow p-12">

            <h1 class="flex justify-center text-3xl font-medium pr-4">Family Box</h1>
            <br>
            <br>

            <!-- Primera columna -->

        <div class="flex-row flex items-center justify-center gap-48">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-14 mr-5 flex flex-col place-items-center">
                    <img alt="Hamburguesa" 
                        src={FamilyBox}
                        class="flex justify-center"
                        height="120"
                        width="120"
                    />
                    <br>
               <div class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white">Hamburgesa</div>
          </div>
        </div>

    </main>
    
    <Footer />
</div>