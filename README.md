# biome-svelte-issues

## src/routes/enumTypeIssue/+page.svelte

Here the is a conflict since Biome doesn't like it when I import without `type`

## src/routes/letBindIssue/MyComponent.svelte

I think this is a known issue but just to have it here, `export let` should be ok and doesn't need a const.

## src/routes/letBindIssue/+page.svelte

If you create a variable that is sent into a component via a `bind` then it can't be const. But Biome complains if it's never modified in this file.