<script>
    let command='';
    let commands = [];
    const handleEnter = () => {
        commands = [...commands, command]
    }
</script>

<form on:submit|preventDefault={handleEnter}>
    <input class=' border rounded py-2 px-3 leading-tight' bind:value={command}>
</form>

{#each commands as cmd}
    <p>{cmd}</p>
{/each}