<script>    
</script>

<nav>
    <button>
        <a href="#">Menu</a>
    </button>
    <ul>
        <li>
            <a href="#">About</a>
        </li>
        <li>
            <a href="#">Work</a>
        </li>
        <li>
            <a href="#">Data</a>
        </li>
        <li>
            <a href="#">Contact</a>
        </li>
    </ul>
</nav>

<style>
    nav{
        text-align: right;
        width: 100%;
        position: fixed;
        background-color: #FFD23F;
        border-bottom: 1px solid black;
        display: flex;
        justify-content: flex-end;
    }

    ul{
        width: 100%;
        list-style: none;
        margin: 1rem 0;
        display: flex;
        justify-content: flex-end;
        margin-right: 1rem;
        
    }

    button{
        background-color: #FFD23F;
        border: none;
        margin: 1rem 0;
        display: none;
        justify-content: flex-end;
        margin-right: 1rem;
        
    }

    li {
        margin: 1rem 1rem;
    }

    a{        border: 1px solid black;
        padding: 1rem;
        text-decoration: none;
        color: black;
        box-shadow: 5px 5px rgba(10, 9, 9, 0.795);
        transition: 0.4s;
        width: 100%;
    }

    a:hover, a:active{
        box-shadow: 1px 1px rgba(17, 15, 15, 0.795);
    }



    @media only screen and (max-width: 500px){
        ul{
            display: none;
        }

        button{
            display: flex;
        }
    }
</style>