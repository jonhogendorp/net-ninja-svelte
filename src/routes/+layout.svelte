<script>
	import Title from '$lib/title.svelte';
	import '../styles/global.css';
</script>

<div class="layout">
	<header>
		<Title />
	</header>
	<main>
		<slot></slot>
	</main>
	<footer>
		<p>&copy; 2024</p>
	</footer>
</div>

<style>
	.layout {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		margin: 20px auto;
		width: 80%;
	}
</style>
