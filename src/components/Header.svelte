<script lang="ts">
	import {base} from "$app/paths";

	function handleClick() {
		alert('My number for donates: 8-800-555-35-35')
	}
</script>

<header>
	<nav>
		<span><b>Menu</b></span>
		<a href="{base}/"><button class="linkbtn">About</button></a>
		<a href="{base}/photos"><button class="linkbtn">Photos</button></a>
		<a href="{base}/contact"><button class="linkbtn">Contact</button></a>
		<button on:click={handleClick} class="donatebtn"> Donate</button>
	</nav>
</header>

<style>
	header {
		background-color: #403d58;
		height: 60px;
	}

	.linkbtn {
		margin-left: 0.5rem;
		margin-top: 0.5rem;
		margin-bottom: 0.5rem;
		font-size: 0.8rem;
		color: #ddabfa;
		cursor: pointer;
		padding: 0.75rem 1.2rem;
		border: 2px solid #ddabfa;
		border-radius: 0.4rem;
		background: transparent;
		font-family: Verdana, sans-serif;
	}

	.linkbtn:hover {
		background-color: #ebe6ea;
		color: #403d58;
		border: 2px solid #403d58;
	}

	.donatebtn {
		margin-left: 0.5rem;
		margin-top: 0.5rem;
		margin-bottom: 0.5rem;
		font-size: 1rem;
		color: #403d58;
		cursor: pointer;
		padding: 0.75rem 1.2rem;
		border: 2px solid #403d58;
		border-radius: 0.4rem;
		background: #edd4ff;
	}

	.donatebtn:hover {
		background-color: #ebe6ea;
	}

	span {
		margin-left: 0.5rem;
		margin-top: 0.5rem;
		margin-bottom: 0.5rem;
		font-size: 1.5rem;
		color: #efe9df;
	}
</style>
