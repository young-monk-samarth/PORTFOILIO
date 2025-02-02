<script>
    export let y;
    export let tabs = [
        { name: "PROJECTS", link: "#projects" },
        { name: "ABOUT ME", link: "#about" },
        { name: "TECHSTACK", link: "#tech" },
        { name: "CONTACT", link: "#connect" },
    ];
</script>

<header class="sticky top-0 z-10 flex items-center justify-between px-4 py-3 md:px-6 md:py-4 duration-200 border-b-2 border-transparent bg-[#0c0a09]">
    <h1 class="text-2xl font-medium md:text-3xl">
        <a href="/" class="font-bold poppi text-gray-100 cursor-pointer relative inline-block group">
            <span class="relative">
                <b>PORT</b>FOLIO
                <span class="absolute bottom-0 left-0 w-0 h-[3px] bg-violet-400 transition-all duration-300 group-hover:w-full"></span>
            </span>
        </a>
    </h1>
    <nav class="hidden items-center gap-4 pr-4 md:flex">
        {#each tabs as { name, link }, i}
            <a href={link} class="duration-200 hover:text-violet-400">
                {name}
            </a>
        {/each}
    </nav>
</header>

<style>
    .poppi {
        font-family: 'Poppins', sans-serif;
    }
</style>