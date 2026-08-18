<script>
	let count = $state(0)
	let factor = $state(0)
	let result = $derived(count * factor)
</script>

<div>
	<h1>{count} * factor = {result}</h1>
	<button onclick={() => count++}>Count: {count}</button>
	<button onclick={() => factor++}>Factor: {factor}</button>
</div>