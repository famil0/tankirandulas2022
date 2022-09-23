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
        background-color: #D9D9D9;
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

    .menu > li > a
    {
        width: 100px;
        background: linear-gradient(45deg, #284B63 0%, #284B63 50%, #3C6E71 50%,  #3C6E71 100%);
        background-size: 230% 100%;
        display: block;
        transition: 0.4s;
    }

    .menu > li > a:hover
    {
        background-position: 100% 0%;
    }

    
    .almenu
    {
        position: absolute;
    }
    
    .almenu > li > a
    {
        display: block;
        width: 100px;
        background: linear-gradient(90deg, #284B63 0%, #284B63 10%, #3C6E71 10%, #3C6E71 100%);
        background-size: 200% 100%;
        transform: translateX(-40%);
        height: 0px;
        transition: 0.4s;
        visibility: hidden;
        /* line-height: 0; */
    }
    
    .menu > li:hover > .almenu > li > a
    {
        /* line-height: 70px; */
        height: 70px;
        visibility: visible;
    }
    
    .almenu > li > a:hover
    {
        /* margin-left: 120%; */
        background-position: -80% 0%;
    }

</style>