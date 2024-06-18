<script lang="ts">
    export let src: string;
    export let alt: string;
    export let classes: string = "";
    export let id: string = "";
    export let hasTransition: boolean = false;

    import IntersectionObserver from "./IntersectionObserver.svelte";
    import Image from "./Image.svelte";
    import { onMount } from "svelte";

    let nativeLoading = false
    // Determine whether to bypass our intersecting check
    onMount(() => {
        if ('loading' in HTMLImageElement.prototype) {
            nativeLoading = true;
        }
    });
</script>

<IntersectionObserver once={true} let:intersecting>
    {#if intersecting || nativeLoading}
        <Image {alt} {src} {classes} {id} {hasTransition} />
    {/if}
</IntersectionObserver>
