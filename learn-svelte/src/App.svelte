<script>

	let obj = {
		src: 'image.gif',
		alt: 'Person nods'
	}

	let lazy = false
</script>

<img {...obj} loading={lazy ? 'lazy' : null} />