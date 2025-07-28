<script>
    import ProjectCard from "$lib/components/ProjectCard.svelte";
</script>

<section class="cards">
    <ul>
        <li>
            <ProjectCard
                    title="Reverb Client"
                    description="A Modern Custom Minecraft PvP Client"
                    image="/images/reverb.png"
                    link=""
            />
        </li>
        <li>
            <ProjectCard
                    title="Reverb Client"
                    description="A Modern Custom Minecraft PvP Client"
                    image="/images/background.png"
                    link=""
            />
        </li>
        <li>
            <ProjectCard
                    title="Reverb Client"
                    description="A Modern Custom Minecraft PvP Client"
                    image="/images/background.png"
                    link=""
            />
        </li>
    </ul>
</section>

<style>
    .cards {
        display: flex;
        justify-content: center;
        align-items: center;
        min-height: 100vh;
        padding: 2rem;
    }

    .cards ul {
        display: flex;
        flex-wrap: wrap;
        gap: 1.5rem;
        justify-content: center;
        align-items: center;
        list-style: none;
        padding: 0;
        margin: 0;
    }
</style>
