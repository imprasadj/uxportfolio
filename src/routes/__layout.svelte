<script>
    import '../global.css';
    
    import { onMount } from 'svelte';
    import Footer from '$lib/Footer.svelte';
    import Navbar from '$lib/Navbar.svelte';
    
    import AOS from 'aos';
    onMount(() => {
		AOS.init()
	})

</script>

<svelte:head>
    <link rel="stylesheet" href="https://unpkg.com/aos@next/dist/aos.css"/>
</svelte:head>

<div class="mainlayout">
    <Navbar/>
    <slot><!-- optional fallback --></slot>
    <Footer/>
</div>

<style>
    .mainlayout{
       background-color: var(--bgcolor);
       z-index: -1; 
   } 
</style>