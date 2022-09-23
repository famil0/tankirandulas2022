<div class="container">
    <slot></slot>
</div>

<style>
    .container
    {
        z-index: -1;
        width: 60%;
        height: 100%;
        background-color: #2EC4B6;
        position: absolute;
        left: 50%;
        transform: translateX(-50%);
        display: grid;
        grid-template-columns: 50% 50%;
        text-align: justify;
    }

    h1
    {
        color: #f700ff;
        grid-column-start: span 2;
    }
</style>