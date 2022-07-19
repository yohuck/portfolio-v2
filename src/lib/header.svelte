<script>    
$: open = false
let handleClick = () => {
    open = !open
    console.log(open)
}


</script>

<nav class={open? 'open' : 'closed'}>

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
    <button on:click={handleClick} class={open? 'openBtn' : 'closedBtn'}>
        <a href="#">{open? 'x' : 'Menu'}</a>
    </button>
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
        align-items: flex-end;
        transition-timing-function: cubic-bezier(0.23, 1, 0.320, 1);
        transition-duration: 1s;
        height: 100%;
        transform: translateY(calc(-100% + 5rem));
    }

    .open {
        transform: translateY(0);
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
        transition: 0.5s;
        transition-timing-function: ease-out;
    }

   .openBtn{
        transform: rotate(1080deg);
        border-radius: 999px;
    }

    li {
        margin: 1rem 1rem;
    }

    a{        border: 1px solid black;
        padding: 1rem;
        text-decoration: none;
        color: black;
        box-shadow: 5px 5px rgba(10, 9, 9, 0.795);
        transition: 0.5s;
        width: 100%;
    }

    a:hover, a:active{
        transition: 0.5s;
        box-shadow: 1px 1px rgba(17, 15, 15, 0.795);
    }
/* 
    a:not(:hover), a:not(:active){
        box-shadow: 5px 5px rgba(10, 9, 9, 0.795);
        transition: 1s;
    } */



    @media only screen and (max-width: 500px){
        ul{
            display: flex;
            flex-direction: column;
            margin: 0rem;
            height: 100%;
            justify-content: flex-start;
        }

        li{
            margin-top: 3rem;
            font-size: 4rem;
            margin-right: -3rem;
        }

        button{
            display: flex;
        }

        a{        border: 1px solid black;
        padding: 1rem;
        text-decoration: none;
        color: black;
        box-shadow: 5px 5px rgba(10, 9, 9, 0.795);
        transition: 0.4s;
        width: 100%;
    }
    }
</style>