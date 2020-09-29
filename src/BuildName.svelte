<script lang="ts">
    let firstName: string = "Akiha";
    let lastName: string = "Arisugawa";
    let fullName: string = `${firstName} ${lastName}`;
</script>

<main>
    <input bind:value={firstName} />
    <input bind:value={lastName} />
    <div>Hello, {fullName}</div>
</main>
