<script>
	import {base} from "$app/paths";
	import Meme from "../components/Meme.svelte";
</script>

<svelte:head>
	<title>Elizaveta Semenova</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<main class="App">
	<div id="main">

		<div class="home-left flex items-center">
			<h4 class="popping">Hi, I'm</h4>
			<h1 class="t-white">Elizaveta Semenova</h1>
<!--			<a href="#" target="_blank">-->
				<button
					class="btn">Resume</button>
<!--			</a>-->
		</div>
		<div class="home-right flex items-center">
			<div class="circle flex items-center" id="mainimage">
				<img src="{base}/lib/images/i.jpg" alt="me">
			</div>
		</div>

		<p>My name is <b>Elizaveta Semenova</b>.
			Right now I'm 3rd year bachelor student of Cyber-security track at Innopolis University. </p>
		<p><u>More information about me you can find in my resume.</u></p>
		<br>
		<p>  </p>
		<h3>Here's a meme:</h3>
		<ul><li>First of all, get a number:</li>
			<li>Then we print the meme:</li>
		</ul>
		<button id="get-meme-btn" class="btn">Get meme!</button>
		<Meme></Meme>
		<br>

	</div>
</main><p><u>More information about me you can find in my resume.</u></p>

<style>
	.home-left,
	.home-right {
		width: 48%;
		padding: 2rem;
	}

	.home-left h1 {
		font-size: 2.5rem;
	}

	.home-right img {
		position: absolute;
		width: 100%;
		left: 10px;
		top: 0;
		background-size: cover;
		border-radius: 62%;
		height: 100%;
	}

	.circle {
		width: 17rem;
		height: 17rem;
		border-radius: 50%;
		padding: .5rem;
		position: relative;
	}

	.about-left img {
		width: 90%;
		border-radius: 1rem;
	}

	.about-content p {
		margin-bottom: 2rem;
	}
</style>