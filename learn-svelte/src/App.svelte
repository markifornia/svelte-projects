<script>
	let content = `
	<h1>Big banana exposed</h1>
	<p>The gorillas inside the banana cartel speak out</p>
	`

</script>

<hgroup>
	{@html content}
</hgroup>

<style lang="postcss">
	hgroup global {
		h1 {
			text-transform: capitalize;
		}

		p {
			color: orangered;
		}
	}

	@keyframes -global-animation {
		/* ... */
	}
</style>