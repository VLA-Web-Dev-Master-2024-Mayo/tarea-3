<script lang="ts">

    // Components
    import Navbar from "$lib/components/Navbar.svelte";
    import Footer from "$lib/components/Footer.svelte";

    // Imágenes
    import MenuHamburguesas from "$lib/assets/Hamburguesas/HamburgesasMenu.png";
    import MenuBebidas from "$lib/assets/Bebidas/BebidasMenu.png";
    import MenuAcompañamientos from "$lib/assets/Acompañamientos/AcompañamientosMenu.png";
    import MenuCajita from "$lib/assets/CajitaFeliz/CajitaMenu.png";
    import MenuHelados from "$lib/assets/Helados/HeladosMenu.png";
    import MenuDesayunos from "$lib/assets/Desayunos/DesayunosMenu.png";
    import MenuCafes from "$lib/assets/McCafes/CafesMenu.png";
    import MenuFamily from "$lib/assets/FamilyBox/FamilyMenu.png";
    
</script>
   
    <Navbar />
    
    <main class="flex-grow p-12 scroll-smooth">

            <h1 class="flex justify-center text-3xl font-medium pr-7">Menú</h1>
            <br>
            <br>

            <!-- Primera columna -->

        <div class="flex-row flex items-center justify-center gap-48">
            
            <div class="border-2 border-yellow-200 bg-white rounded-md p-16 px-20 flex flex-col place-items-center">
                    <img alt="Menú Hamburgesas" 
                        src={MenuHamburguesas}
                        class="flex justify-center"
                    />
                    <br>
                    <a href="/hamburguesas">
                        <button class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white hover:text-black hover:bg-white">Hamburguesas</button>
                    </a>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-16 mr-9 flex flex-col place-items-center">
                    <img alt="Menú Bebidas" 
                        src={MenuBebidas}
                        class="flex justify-center"
                    />
                    <br>
                    <a href="/bebidas">
                        <button class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white hover:text-black hover:bg-white">Bebidas</button>
                    </a>
            </div>

            <div class="border-2 border-yellow-200 bg-white rounded-md p-16 flex flex-col place-items-center">
                    <img alt="Menú Acompañamientos" 
                        src={MenuAcompañamientos}
                        class="flex justify-center"
                    />
                    <br>
                    <a href="/acompañamientos">
                        <button class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white hover:text-black hover:bg-white">Acompañamientos</button>
                    </a>
            </div>
        </div>

        <br>
        <br>
        <br>

        <!-- Segunda columna -->

        <div class="flex-row flex items-center justify-center gap-80">
            <div class="border-2 border-yellow-200 bg-white rounded-md p-16 flex flex-col place-items-center">
                    <img alt="Menú Cajiita Feliz" 
                        src={MenuCajita}
                        class="flex justify-center"
                    />
                    <br>
                    <a href="/cajita">
                        <button class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white hover:text-black hover:bg-white">Cajita Feliz</button>
                    </a>
            </div>

             <div class="border-2 border-yellow-200 bg-white rounded-md p-16 mr-6 flex flex-col place-items-center">
                    <img alt="Menú Helados" 
                        src={MenuHelados}
                        class="flex justify-center"
                    />
                    <br>
                    <a href="/helados">
                        <button class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white hover:text-black hover:bg-white">Helados</button>
                    </a>
            </div>

             <div class="border-2 border-yellow-200 bg-white rounded-md p-16 flex flex-col place-items-center">
                    <img alt="Menú Desayunos" 
                        src={MenuDesayunos}
                        class="flex justify-center"
                    />
                    <br>
                    <a href="/desayunos">
                        <button class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white hover:text-black hover:bg-white">Desayunos</button>
                    </a>
            </div>
        </div>

        <br>
        <br>
        <br>

        <!-- Tercera columna -->
        
        <div class="flex-row flex items-center justify-center gap-80">
            <div class="border-2 border-yellow-200 bg-white rounded-md p-16 flex flex-col place-items-center">
                    <img alt="Menú Cafés" 
                        src={MenuCafes}
                        class="flex justify-center"
                    />
                    <br>
                    <a href="/cafes">
                        <button class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white hover:text-black hover:bg-white">Cafés</button>
                    </a>
            </div>

           <div class="border-2 border-yellow-200 bg-white rounded-md p-16 flex flex-col place-items-center">
                    <img alt="Menú Family Box" 
                        src={MenuFamily}
                        class="flex justify-center"
                    />
                    <br>
                    <a href="/family">
                        <button class="p-2 border-2 border-yellow-300 bg-yellow-300 rounded-full text-white hover:text-black hover:bg-white">Family Box</button>
                    </a>
            </div>

        </div>

    </main>
    
    <Footer />