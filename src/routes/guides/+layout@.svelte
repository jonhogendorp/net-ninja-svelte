<script>
	import Title from '$lib/title.svelte';
	import '../../styles/global.css';
</script>

<div class="layout">
	<header>
		<Title title="Johnny`s gaming guide " />
		<div class="links">
			<a href="/">Home</a>
			<a href="/about"> About </a>
			<a href="/guides"> guides </a>
		</div>
	</header>
	<main>
		<slot />
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
	.links {
		margin-left: auto;
	}
	a {
		margin-left: 10px;
	}
</style>
