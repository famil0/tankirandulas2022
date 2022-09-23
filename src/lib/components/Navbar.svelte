<div class="container">
    <ul class="menu">
        <li><a>Napok</a>
            <ul class="almenu">
                <li><a href="../../nap/1/">1. nap</a></li>
                <li><a href="../../nap/2/">2. nap</a></li>
                <li><a href="../../nap/3/">3. nap</a></li>
            </ul>
        </li>
        <li><a href="">Szolo</a></li>
        <li><a href="">Korte</a></li>
    </ul>
</div>
<style>

    .container
    {
        background-color: #2EC4B6;
        display: grid;
        justify-content: center;
        align-content: center;
    }
    
    ul
    {
        list-style: none;
        
    }

    a
    {
        color: white;
        /* display: inline-block; */
    }

    li
    {
        /* height: 70px; */
        line-height: 70px;
        text-align: center;
    }

    .menu > li
    {
        display: inline-block;
    }

    .menu > li
    {
        width: 100px;
        background: linear-gradient(45deg, #FF9F1C 0%, #FF9F1C 50%, #FFBF69 50%,  #FFBF69 100%);
        background-size: 230% 100%;
        transition: 0.4s;
    }

    .menu > li:hover
    {
        background-position: 100% 0%;
    }

    
    .almenu
    {
        position: absolute;
    }
    
    .almenu > li
    {
        display: block;
        width: 100px;
        background: linear-gradient(90deg, #FF9F1C 0%, #FF9F1C 10%, #FFBF69 10%, #FFBF69 100%);
        background-size: 200% 100%;
        transform: translateX(-40%);
        height: 0px;
        transition: 0.4s;
        visibility: hidden;
        /* line-height: 0; */
    }
    
    .menu > li:hover > .almenu > li
    {
        height: 70px;
        visibility: visible;
    }
    
    .almenu > li:hover
    {
        /* margin-left: 120%; */
        background-position: -80% 0%;
    }

</style>