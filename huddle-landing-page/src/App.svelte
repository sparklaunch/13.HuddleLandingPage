<script lang="ts">
    let innerWidth: number;
    $: isMobile = innerWidth <= 1440;
    $: document.body.id = isMobile ? "mobile-body" : "desktop-body";
</script>

<svelte:window bind:innerWidth />
<div id="app" />
