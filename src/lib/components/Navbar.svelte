<script>
import NavButton from "$lib/components/NavButton.svelte";
</script>

<nav class="navbar">
    <ul>
        <NavButton name="Home" page="" />
        <NavButton name="Projects" page="projects" />
        <NavButton name="Contact" page="contact" />
    </ul>
</nav>

<style>
    .navbar {
        position: absolute;
        top: 0;
        right: 0;
        padding: 1rem;
        display: flex;
        gap: 1rem;
        font-family: 'Syne', sans-serif;
    }
</style>