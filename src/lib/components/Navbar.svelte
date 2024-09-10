<script lang="ts">
    type Menu={title:String;page_link:string};

    const menu:Menu[]=[{title:"Productos",page_link:"/src/routes/productos/+page.svelte"},
                       {title:"Restaurantes",page_link:"1"},
                       {title:"En Familia",page_link:"1"},
                       {title:"Nosotros",page_link:"1"},
                       {title:"McDelivery",page_link:"1"},
                       {title:"Cupones",page_link:"1"},
    ];

</script>

<nav class="bg-#ffffff shadow-lg w-full flex justify-center gap-1">
    <img src="/assets/mcdonalds-logo-footer-bg-white.png" alt="logo" class="h-[140px]">
    <ul class="flex justify-center items-end  h-32 gap-5 font-speedee font-normal">
        {#each menu as item }
            <li class="hover:border-b-4 hover:border-yellow-500 h-10"><a href={item.page_link} class="p-4">{item.title}</a></li>
        {/each}

    </ul>
</nav>


