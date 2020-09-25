<script>
	import * as S from "svelte-materialify/src/";
	
	let theme = 'light';
	
	function toggleTheme() {
		if (theme === 'light') theme = 'dark';
		else theme = 'light';
	}
</script>

<S.MaterialApp {theme}>
	<S.AppBar>
		<span slot="title">Title</span>
	</S.AppBar>
	<br />
	<h2 class="mb-4">
		Svelte Materialify
	</h2>
	<S.Divider />
	<br>
	<div class="text-center">
		<a href="//github.com/TheComputerM/svelte-materialify/stargazers">
			<S.Button class="primary-color">
				Star on GitHub
			</S.Button>
		</a>
		<S.Button on:click={toggleTheme}>Toggle Theme</S.Button>
	</div>
	<br />
</S.MaterialApp>