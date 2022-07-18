<script>

    let skills = [
        {
            id: 1,
            name: "HTML"
        },
        {
            id: 2,
            name: "Javascritp"
        }
    ]
</script>

<div class="Skills">
    {#each skills as {name}, i}
        <li>{name}</li>
    {/each}
</div>