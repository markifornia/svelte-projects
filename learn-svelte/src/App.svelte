<script>
	let count = $state(0)
	let max = $derived(count >= 4)

	$inspect(max)
</script>

<div>
	<button onclick={() => count++} disabled={max}>Count: {count}</button>
</div>