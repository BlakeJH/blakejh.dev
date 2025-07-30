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
                    link="https://github.com/LofizKittyCat/ReverbClient"
            />
        </li>
        <li>
            <ProjectCard
                    title="NoHurtCam+"
                    description="A Minecraft NoHurtCam Mod For 1.19 - 1.20.2"
                    image="/images/nohurtcam.png"
                    link="https://modrinth.com/mod/nohurtcam+"
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
