<script>
	function validate() {
		console.log("I'm the validate() function")
	}

    import contactToggle from './svgs.svelte'

    console.log(contactToggle)
</script>

<div class="contact_container" id={toggler? "off" : "on"}>
    <form on:submit|preventDefault={validate}>
        <h1>Take me to your leader</h1>
        <p>(As long as they're hiring)</p>
        Email Address:
        <input>
        Message:
        <textarea  cols="30" rows="10"></textarea>
        <button type="submit">
            Submit
        </button>
    </form>
</div>

<style>
    form{
        display: flex;
        flex-direction: column;

    }

    button{
        padding: 0.75em;
        font-family: monospace;
        border: none;
        font-weight: 900;
        color: white;
        background-color: #3BCEAC;
       margin: 1rem auto;
        max-width: 100px;
    }

    .contact_container{
        position: fixed;
        width: 80%;
        max-width: 300px;
        margin: 0 auto;
        background-color: #FFD23F;
        z-index: 20;
        padding: 2rem;
        border-radius: 2px;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);
        box-shadow: 10px 10px rgba(78, 77, 77, 0.795);
        transition: 3s;
    }

    #off{
        transform: translate(-50%, 300%);
        transition: 3s;
    }

    h1{
        margin-bottom: 0;
    }
</style>