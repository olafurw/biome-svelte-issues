<script lang="ts">
    // I think you know about this one, marked in your partial svelte support
    // But let should be ok if its "export let"
    export let value: number | undefined = undefined;
</script>

<div>
    {value}
</div>