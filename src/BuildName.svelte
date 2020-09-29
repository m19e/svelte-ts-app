<script lang="ts">
    let firstName: string = "Akiha";
    let lastName: string = "Arisugawa";
    $: fullName = `${firstName} ${lastName}`;
</script>

<main>
    <input bind:value={firstName} />
    <input bind:value={lastName} />
    <div>Hello, {fullName}</div>
</main>
