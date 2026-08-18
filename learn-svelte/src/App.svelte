<script>
	let open = $state(false)
</script>

<button onclick={() => open = !open} class="btn">
	<span>Item A</span>
	<span class={['trigger', { open }]}>👈</span>
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