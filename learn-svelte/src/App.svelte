<script>
	let open = $state(false)
</script>

<button onclick={() => open = !open} clas="btn">
	<span>Item A</span>
	<span class="trigger" class:open>👈</span>
</button>

<style>
	.trigger {
		display: inline-block;
		transition: rotate 0.2s ease;

		&.open {
		rotate: -90deg;
	}
	}
</style>