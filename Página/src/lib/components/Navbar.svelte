<script>
    import Logo2 from "$lib/assets/Logos/Logo2.png";
</script>

<nav class="bg-yellow-500 p-4 text-2xl">
    <div class="flex justify-center">  
            <div class="flex-grow">
                <a href="/" class="flex w-16 h-16">
                    <img alt="Logo McDonals" 
                        src={Logo2}
                        height="65"
                        width="65"
                        class="flex justify-start hover:shadow-md hover:shadow-red-900 transition-all duration-400"
                    />
                </a>
            </div>

            <div class="flex flex-grow items-center">
                <a href="/">
                    <span class="material-symbols-outlined text-3xl border-b-2 text-white hover:animate-pulse hover:text-4xl transition-all duration-300">
                        home
                    </span>
                </a>
            </div>
            
        <a href="/menu" class="flex items-center">
            <button class="flex gap-1 border-2 border-white rounded-2xl text-white p-2 hover:shadow-black shadow-md hover:text-black hover:bg-white transition-all duration-300">
                <h1 class="flex">Menú</h1>
                <span class="material-symbols-outlined text-2xl">
                    fastfood
                </span>
            </button>
        </a>
    </div>
</nav>