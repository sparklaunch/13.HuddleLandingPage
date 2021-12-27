<script lang="ts">
    import Logo from "./components/Logo.svelte";
    import Content from "./components/Content.svelte";
    import Footer from "./components/Footer.svelte";
    let innerWidth: number;
    $: isMobile = innerWidth <= 1440;
    $: document.body.id = isMobile ? "mobile-body" : "desktop-body";
</script>

<svelte:window bind:innerWidth />
<main>
    <div id="container">
        <Logo />
        <Content />
        <Footer />
    </div>
</main>

<style>
    main {
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    #container {
        display: flex;
        flex-direction: column;
        width: 80%;
    }
    @media all and (max-width: 1440px) {
        main {
            height: auto;
            display: block;
            padding: 50px 0;
        }
        #container {
            width: 90%;
            margin: auto;
        }
    }
</style>
