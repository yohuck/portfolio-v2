<script>   

import {contactOpen} from '../../src/stores'

// $: contactRead = contactOpen.subscribe(n => console.log(n))

$: open = false
let handleClick = () => {
    open = !open
    console.log(open)
}




let openContact = () => {
    let mql = window.matchMedia('(max-width: 500px)');
    mql.matches? contactOpen.set(!open) : contactOpen.set(open)
    mql.matches? open=!open : open =open
}





let closeDrawer = () => {
    let mql = window.matchMedia('(max-width: 500px)');
    console.log(mql)
    mql.matches? open=!open : open =open
}


</script>

<nav class={open? 'open' : 'closed'}>

    <ul>
        <li>
            <a href="#about" on:click={closeDrawer}>About</a>
        </li>
        <li>
            <a href="#work" on:click={closeDrawer}>Work</a>
        </li>
        <li>
            <a href="#data" on:click={closeDrawer} >Stack</a>
        </li>
        <li>
            <a href="#" on:click={openContact}>Contact</a>
        </li>
    </ul>
    <button on:click={handleClick} class={open? 'openBtn' : 'closedBtn'}>
        <a href="#">{open? 'x' : 'Menu'}</a>
    </button>
</nav>

<style>
    nav{
        z-index: 10;
        text-align: right;
        width: 100%;
        position: fixed;
        background-color: #ffd23ff6;
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
            font-size: 3rem;
            margin-right: -3rem;
        }

        button{
            display: flex;
        }

        a{       
            box-sizing: border-box;
             border: 2px solid black;
        padding: 1rem;
        text-decoration: none;
        color: black;
        box-shadow: 5px 5px rgba(10, 9, 9, 0.795);
        transition: 0.4s;
        width: 100%;
    }
    }
</style>