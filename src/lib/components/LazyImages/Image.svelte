<script lang="ts">
    export let src: string;
    export let alt: string;
    export let classes: string;
    export let id: string;
    export let hasTransition: boolean;

    import { onMount } from "svelte";

    let loaded = false;
    let thisImage: HTMLImageElement;

    onMount(() => {
        thisImage.onload = () => {
            loaded = true;
        };
    });
</script>

{#if id !== ""}
    <img
        {src}
        {alt}
        class="{classes} {loaded ? 'loaded' : ''} {hasTransition ? 'transition' : ''}"
        {id}
        bind:this={thisImage}
        loading="lazy"
    />
{:else}
    <img
        {src}
        {alt}
        class="{classes} {loaded ? 'loaded' : ''} {hasTransition ? 'transition' : ''}"
        bind:this={thisImage}
        loading="lazy"
    />
{/if}

<style>
    img.transition {
        opacity: 0;
        transition: opacity 4000ms ease-out;
    }
    img.transition.loaded {
        opacity: 1;
    }
</style>
