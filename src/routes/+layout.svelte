<script lang="ts">
    import Header from "./Header.svelte";
    import "../app.css";
    import "../images.css";
    import Footer from "./Footer.svelte";
</script>

<!-- <svelte:head>
    <link rel="stylesheet" href="fonts.css" />
</svelte:head> -->

<div class="layout">
    <Header />

    <main>
        <slot />
    </main>

    <Footer />
</div>