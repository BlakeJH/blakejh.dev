<script>
    import NavButton from "$lib/components/NavButton.svelte";
</script>

<div class="navbar">
    <div class="nav-inner w-[730px] h-[60px] bg-neutral-900 rounded-[20px]">
        <div class="icon">
            <NavButton icon="ic:baseline-home" page="urmom" />
            <NavButton icon="ic:baseline-settings" page="urmom" />
            <NavButton icon="ic:baseline-settings" page="urmom" />
            <NavButton icon="ic:baseline-settings" page="urmom" />
            <NavButton icon="ic:baseline-settings" page="urmom" />
        </div>
    </div>
</div>

<style>
    .navbar {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-top: 15px;
    }

    .nav-inner {
        background-color: #111111;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 60px;
    }

    .icon {
        color: white;
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        gap: 50px;
    }
</style>
