<script>
    import { dfx_svelte_poc_backend as canister } from "../../declarations/dfx_svelte_poc_backend";

    let name = "";
    let response = "";

    function handleBtnClick() {
        response = "waiting ...";
        canister.greet(name).then((r)=>response=r);
        name = "";
    }


</script>
<img src="logo2.svg" alt="DFINITY logo" />
<label for="name">Enter your name: &nbsp;</label>
<input id="name" alt="Name" type="text" bind:value={name}/>
<button on:click={handleBtnClick}>Click Me!</button>
<p>{response}</p>  
<p>Visit the <a href="https://internetcomputer.org/docs/current/developer-docs/ic-overview">Internet Computer documentation</a> Home of documentation and developer resources for the Internet Computer (IC)</p>
