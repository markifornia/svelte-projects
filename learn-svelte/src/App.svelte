<script>
	let color = 'orangered'
</script>

<h1 style="--color: {color}">Svelte</h1>

<h1 style:--color={color}>Svelte</h1>

<style>
	h1 {
		color: var(--color, #fff);
	}
</style>

