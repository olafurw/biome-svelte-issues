<script lang="ts">

    // This line makes biome happy but svelte complains in the HTML section
    import type { MyEnum } from "$lib/types";

    // This line makes svelte happy but biome complains
    // All these imports are only used as types.biomelint/style/useImportType
    // import { MyEnum } from "$lib/types";

    const value: MyEnum | undefined = undefined;
</script>

<div>
    {#if value === MyEnum.A}
        A
    {:else if value === MyEnum.B}
        B
    {:else}
        C
    {/if}
</div>