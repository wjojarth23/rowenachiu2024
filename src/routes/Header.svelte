<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/svelte-logo.svg';
	import github from '$lib/images/github.svg';
</script>

<header>
		<ul>
			<div>
				<a href="/">Home</a>
			</div>
			<div>
				<a href="/about">About</a>
			</div>
			<div>
				<a href="/priorities">Priorities</a>
			</div>
		</ul>
</header>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
	header {
		display: flex;
		width:100%;
		height:100px;
		justify-content:center;
	  background: #e03539;
	}


	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 100%;
		margin-right: 0;
		margin-left:auto;
		display: flex;
		align-items: center;
		list-style: none;
		
	}

	div {
		font-family: "Poppins", sans-serif;
  font-weight: 500;
  font-style: normal;
	font-size:20px;
		position: relative;
		height: 100%;
		justify-content: center;
		align-items: center;
		margin:20px;
		line-height: 100px;
  	text-align: center;
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

</style>
