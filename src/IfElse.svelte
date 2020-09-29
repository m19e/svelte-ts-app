<script lang="ts">
    export let checked: boolean = false;
</script>

<label> <input type="checkbox" bind:checked /> Raise the Sun! </label>
{#if checked}
    <div>Day!!!!</div>
{:else}
    <div>Night....</div>
{/if}
