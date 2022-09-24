<div class="header"><h1><a href="../../">Tanulmányi kirándulás 2022</a></h1></div>
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


    .header
    {
        height: 70px;
        width: 100%;
        text-align: center;
        display: flex;
        justify-content: center;
        line-height: 70px;   
        z-index: 1;
        position: sticky;
        top: 0;
    }

    .header > h1 > a
    {
        color: #CBF3F0;
        text-shadow: 2px 2px 2px black;
        transition: 0.4s;
    }

    .header > h1 > a:hover
    {
        font-size: 1.1em;
    }

    .container, .header
    {
        background: linear-gradient(90deg, #11ebd5 0%, #2EC4B6 20%, #2EC4B6 20%, #2ec486 80%, #2ec486 80%, #2ec42e 100%);
    }

    .container
    {
        display: grid;
        justify-content: center;
        align-content: center;
        padding-bottom: 1.5%;
    }
    
    ul
    {
        list-style: none;
        
    }

    a
    {
        color: white;
        display: block;        
    }

    li
    {
        line-height: 70px;
        text-align: center;
    }
    
    .menu > li
    {
        display: inline-block;
        width: 100px;
        background: linear-gradient(45deg, #FF9F1C 0%, #FF9F1C 50%, #FFBF69 50%,  #FFBF69 100%);
        background-size: 230% 100%;
        transition: 0.4s;
    }

    .menu > li:hover
    {
        background-position: 100% 0%;
    }

    .menu
    {
        z-index: 0;
        overflow: hidden;
    }
    
    .almenu
    {
        position: absolute;
        z-index: -1;
        visibility: hidden;
        transform: translateY(-100%);
        transition: 0.4s;
    }
    
    .almenu > li
    {
        width: 100px;
        background: linear-gradient(90deg, #FF9F1C 0%, #FF9F1C 10%, #FFBF69 10%, #FFBF69 100%);
        background-size: 200% 100%;
        transform: translateX(-40%);
        transition: 0.4s;
    }

    .almenu > li > a
    {
        transition: 0.4s;
        margin-left: 20%;
    }

    .menu > li:hover > .almenu
    {
        visibility: visible;
        transform: translateY(-0%);
    }
    
    .almenu > li:hover
    {
        background-position: -80% 0%;
    }

    .almenu > li:hover > a
    {
        margin-left: -20%;
    }

</style>