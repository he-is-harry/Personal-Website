<script>
    import ImageLoader from "$lib/components/LazyImages/ImageLoader.svelte";
</script>

<div class="content">
    <h1>Thanks for emailing Harry!</h1>
    <h2>Harry will try to reply as soon as he is avaliable.</h2>
    <br />

    <p class="notice">Note: Harry does not check this website's email that often, in order to reach out to him more urgently, contact him on <a href="https://ca.linkedin.com/in/harryghe">Linkedin</a>.</p>
    <ImageLoader classes="thanks-image" src="/Thanks.gif" alt="Thank you"></ImageLoader>
    <!-- <img src="/Thanks.gif" alt="Thank you" class="thanks-image"/> -->
</div>

<svelte:head>
    <title>Thanks</title>
</svelte:head>


<style>
    .content {
        margin-inline: var(--size-6);
    }
</style>
