<script>
	function validate() {
		console.log("I'm the validate() function")
	}
</script>

<form on:submit|preventDefault={validate}>
	Email Address:
    <input>
    Message:
    <textarea  cols="30" rows="10"></textarea>
	<button type="submit">
		Submit
	</button>
</form>

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
</style>