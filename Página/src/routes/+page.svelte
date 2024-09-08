<script lang="ts">

// Components
import Navbar from "$lib/components/Navbar.svelte";
import Footer from "$lib/components/Footer.svelte";

</script>

<div class="flex flex-col min-h-screen max-w-full justify-center">
    <Navbar />

    <main class="flex-grow">
        <section class="bg-cover">
            <img src="https://cdn.pixabay.com/photo/2019/10/22/18/49/mcdonalds-4569513_1280.jpg" alt="Letrero McDonald´s">
            <img src="https://cdn.pixabay.com/photo/2024/03/01/11/08/ai-generated-8606255_1280.jpg" alt="Hamburguesa Big Mac">
            <img src="https://cdn.pixabay.com/photo/2016/11/22/23/23/french-fries-1851143_1280.jpg" alt="Chica comiendo McPapas">
            <img src="https://cdn.pixabay.com/photo/2023/09/23/15/56/ai-generated-8271284_1280.jpg" alt="Hamburguesa Cuarto de libra">
            <img src="https://cdn.pixabay.com/photo/2017/06/07/06/35/beijing-airport-2379526_1280.jpg" alt="Reustaurante McDonald´s">
        </section>
    </main>

    <Footer />
</div>