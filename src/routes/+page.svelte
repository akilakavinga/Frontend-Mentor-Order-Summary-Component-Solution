<script>
    import OrderSummary from "$lib/components/OrderSummary.svelte";
    import Attribution from "../lib/components/Attribution.svelte";
</script>

<main>
    <OrderSummary />
    <Attribution />
</main>

<style lang="scss">
    @use "$lib/styles" as *;

    :global(*, *::after, *::before) {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        font-family: $redHatDisplay;
    }

    :global(body) {
        font-size: $bodyFz;
        height: 100vh;
        background-color: $paleBlue;
        @include flexCol;
    }

    main {
        height: 100%;
        position: relative;
        @include flexCol;
    }
</style>
