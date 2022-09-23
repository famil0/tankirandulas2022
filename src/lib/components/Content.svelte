<div class="container">
    <slot></slot>
</div>

<style>
    .container
    {
        z-index: -1;
        width: 60%;
        background-color: #2EC4B6;
        position: absolute;
        left: 50%;
        transform: translateX(-50%);
        display: grid;
        grid-template-columns: 50% 50%;
        text-align: justify;
        min-width: 450px;
    }

    .container > :global(h1), :global(h4)
    {
        grid-column-start: span 2;
        text-align: center;
    }

    .container > :global(p)
    {
        margin-bottom: 10%;
        grid-column-start: 1;
    }

    .container > :global(h3)
    {
        grid-column-start: 1;
    }
    
    .container > :global(p), :global(h2), :global(h3)
    {
        margin-left: 10%;
    }

    .container > :global(h3), :global(h4)
    {
        margin-bottom: 2%;
    }

    .container > :global(img)
    {
        width: 60%;
        margin: 0 auto 10% auto;
    }
</style>