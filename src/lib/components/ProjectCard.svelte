<script lang="ts">
    export let title: string = "";
    export let description: string = "";
    export let image: string = "";
    export let link: string = "#";
</script>

<a class="glass-card" href={link} target="_blank" rel="noopener noreferrer">
    <div style="padding: 16px; color: white;">
        {#if image}
            <img src={image} alt={title} style="width: 100%; border-radius: 12px; margin-bottom: 12px;" />
        {/if}
        {#if title}
            <h3 style="margin: 0 0 8px 0; font-size: 1.1rem;">{title}</h3>
        {/if}
        {#if description}
            <p style="margin: 0; font-size: 0.9rem; line-height: 1.2rem; color: rgba(255,255,255,0.8);">
                {description}
            </p>
        {/if}
    </div>
</a>

<style>
    .glass-card {
        width: 240px;
        height: 360px;
        background: rgba(255, 255, 255, 0.05);
        backdrop-filter: blur(20px);
        -webkit-backdrop-filter: blur(20px);
        border-radius: 20px;
        border: 1px solid rgba(255, 255, 255, 0.3);
        box-shadow:
                0 8px 32px rgba(0, 0, 0, 0.1),
                inset 0 1px 0 rgba(255, 255, 255, 0.5),
                inset 0 -1px 0 rgba(255, 255, 255, 0.1),
                inset 0 0 0px 0px rgba(255, 255, 255, 0);
        position: relative;
        overflow: hidden;
        text-decoration: none;
        display: block;
    }

    .glass-card::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        height: 1px;
        background: linear-gradient(
                90deg,
                transparent,
                rgba(255, 255, 255, 0.8),
                transparent
        );
    }

    .glass-card::after {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 1px;
        height: 100%;
        background: linear-gradient(
                180deg,
                rgba(255, 255, 255, 0.8),
                transparent,
                rgba(255, 255, 255, 0.3)
        );
    }
</style>
