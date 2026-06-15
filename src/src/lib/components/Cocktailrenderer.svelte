<script>
    import Cocktail from '$lib/components/Cocktail.svelte';
    const { cocktails } = $props();
</script>

<main class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 2xl:grid-cols-5 gap-6 p-6 max-w-[1600px] mx-auto bg-[#f4f4f9] min-h-screen content-start">
    {#each cocktails as cocktail}
        <Cocktail {cocktail}></Cocktail>
    {/each}
</main>