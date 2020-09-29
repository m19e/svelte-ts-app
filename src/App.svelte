<script lang="ts">
    import Greet from "./Greet.svelte";
    import Card from "./Card.svelte";
    import BuildName from "./BuildName.svelte";
    import IfElse from "./IfElse.svelte";
    import Each from "./Each.svelte";
    import Bar from "./Bar.svelte";
    export let name: string;
    let checked: boolean = false;
</script>

<style lang="scss">
    main {
        text-align: center;
        padding: 1em;
        max-width: 240px;
        margin: 0 auto;
        background-color: rgb(200, 200, 200);
        p {
            color: #ff3e00;
        }
    }

    @media (min-width: 640px) {
        main {
            max-width: none;
        }
    }
</style>

<main>
    <Card>
        <Greet {name} />
    </Card>
    <p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
    <input placeholder="Enter your name" bind:value={name} />
    <div>Hello, {name}</div>
    <div><input type="checkbox" bind:checked /> current status is [{'' + checked}]</div>
    <BuildName />
    <IfElse {checked} />
    <Each />
    <Bar label="HP" value={200} />
</main>
