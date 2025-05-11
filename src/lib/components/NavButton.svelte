<script lang="ts">
    import Icon from "@iconify/svelte";
    import {goto} from "$app/navigation";
    export let icon;
    export let page: string;

    function handleClick() {
        goto('/' + page);
    }
</script>

<div
        on:click={handleClick}
        class="transition-transform hover:-translate-y-2 duration-300 cursor-pointer"
>
    <Icon icon={icon} width={50} height={50} />
</div>



