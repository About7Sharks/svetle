<script>
	export let name;
	let pic= '../jhc.svg'
</script>

<main>
	<div id="text">
	<h1>Hello {name} :D!!</h1>
	<img id="mePic" src={pic} alt=""><br>
	<p><strong>Svelte</strong> is a new approach to building user interfaces. Whereas traditional frameworks like React and Vue do the bulk of their work in the browser, Svelte shifts that work into a compile step that happens when you build your app.
	Instead of using techniques like virtual DOM diffing, Svelte writes code that surgically updates the DOM when the state of your app changes.</p>
	<span><a target="_blank" href="https://github.com/About7Sharks?tab=repositories">Git</a> | <a target="_blank" href="http://about7sharks.com/about">About Me</a> | <a target="_blank" href="https://www.linkedin.com/in/zachary-carlin-85402a123/">Linkedin</a></span>
	</div>
</main>

<style>

@keyframes gradientBG {
    0% {
        background-position: 0% 50%;
    }
    50% {
        background-position: 100% 50%;
    }
    100% {
        background-position: 0% 50%;
    }
}
	main {
		display: flex;
		align-items: center; 
		justify-content: center;
		text-align: center;
		position: absolute;
		margin: 0 auto;
		width: 100%;
		height: 100%;
		font-family: "Exo", sans-serif;
		color: #fff;
		background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
		background-size: 400% 400%;
		animation: gradientBG 15s ease infinite;
	}
	#text{
		text-align: center;
		margin: 0 auto;
		background: rgba(233, 233, 231, 0.233);
		padding: 5px;
		margin: 15px;
		width: 80%;
		max-width: 600px;
		border-radius: 20px;
		box-shadow: 3px 3px 3px rgba(0, 0, 0, 0.075);
	}
	#text:hover{
	   box-shadow: 0 0 rgba(0, 0, 0, 0.075);
	   transition: 1s;
	}
	#mePic{
		width: 200px;
		height: 200px;
	}

	h1 {
		color: black;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
		margin: 0;
	}
	p{
		padding: 15px;
		color: #000000;
	}
	a{
		color: #000000;
	}

	@media (max-width: 640px) {
		main {
			height: auto;
		}
	}
</style>