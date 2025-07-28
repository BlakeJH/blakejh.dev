<script lang="ts">
    import { goto } from "$app/navigation";

    export let name: string;
    export let page: string;

    function handleClick() {
        goto('/' + page);
    }
</script>

<button
        on:click={handleClick}
        aria-label={"Navigate to " + page}
        type="button"
        class="frosted-button"
>
    {name}
</button>

<style>
    .frosted-button {
        background: rgba(255, 255, 255, 0.15);
        backdrop-filter: blur(10px);
        -webkit-backdrop-filter: blur(10px);
        border-radius: 40px;
        border: 1px solid rgba(255, 255, 255, 0.3);
        color: white;
        padding: 10px 28px;
        font-weight: 600;
        cursor: pointer;
        transition: background 0.3s ease, box-shadow 0.3s ease;
        user-select: none;
        outline: none;
        margin-left: 5px;
        margin-right: 5px;
    }

    .frosted-button:hover,
    .frosted-button:focus {
        background: rgba(255, 255, 255, 0.3);
        box-shadow: 0 0 12px rgba(255, 255, 255, 0.5);
    }

    .frosted-button:active {
        box-shadow: 0 0 8px rgba(255, 255, 255, 0.3);
    }

</style>
