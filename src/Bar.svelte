<script lang="ts">
    export let label: string = "";
    export let value: number = 0;
</script>

<style>
    .container {
        display: flex;
        align-items: center;
        height: 1.5em;
        padding: 0.2em 0;
    }

    .label {
        margin-right: 0.5em;
        width: 4em;
        text-align: right;
    }

    .bar {
        background-color: white;
        height: 100%;
        width: var(--value, 0);
    }
</style>

<div class="container">
    <div class="label">{label}</div>
    <div class="bar" style="--value: {value}px" />
</div>
