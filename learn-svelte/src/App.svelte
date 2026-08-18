<script>
	let status = $state('closed')
</script>

<button class="btn">
	<span>Item A</span>
	<span class="trigger" data-status={status}>👈</span></button>
<style>
	.trigger {
		display: inline-block;
		transition: rotate 0.2s ease;

		&[data-status='open'] {
			rotate: -0deg;
		}
	}
</style>