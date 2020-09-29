<script lang="ts">
    export let checked: boolean = false;
</script>

<div>
    <label> <input type="checkbox" bind:checked /> Check Me! </label>
    {#if checked}
        <div>Checked!</div>
    {:else}
        <div>Hurry!!</div>
    {/if}
</div>
