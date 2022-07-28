<script lang="ts">
    import { onMount } from 'svelte'

    import init, { greet } from './../../static/wasm.js'

    onMount(async () => {
        await init()
    })
</script>

<button class="bg-red-300 m-4 p-4 rounded text-lg" on:click={greet}>
    🦀 + 🕸 Hello WebAssembly!
</button>