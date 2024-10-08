<script>
	import Header from './Header.svelte';
	import '../app.css';
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>
<footer>

ROWENA CHIU

- FOR PALO ALTO SCHOOL BOARD -

Facebook
Instagram
Threads  
TikTok
X   
Paid For By Rowena Chiu for Palo Alto School Board 2024 FPPC ID #1471019


voterowenachiu@gmail.com

(202) 378-8689
</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height:100px;
		background:#383838;
		color:white;
	}

	footer a {
		font-weight: bold;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
