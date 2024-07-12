<script lang="ts">
    import MyComponent from "./MyComponent.svelte";

    // This line makes svelte happy, since bind can't be used on const variables
    // But biome complains: This let declares a variable that is only assigned once.biomelint/style/useConst
    // let value: number | undefined = undefined;

    // This line makes biome happy, but svelte complains
    const value: number | undefined = undefined;
</script>

<MyComponent bind:value />