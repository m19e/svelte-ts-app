<script lang="ts">
    const persons: { [key: string]: string }[] = [{ name: "Alice" }, { name: "Bob" }, { name: "Carol" }];
</script>

{#each persons as { name }}
    <div>{name}</div>
{/each}
