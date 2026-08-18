<script>
	let { theme, content } = $state({
		theme: 'dark',
		content: '<h1>Svelte</h1>'
	})
</script>

<textarea
	class="editor"
	value={content}
	oninput={(e) => {
		content = e.target.value
	}}
	spellcheck="false"
></textarea>

{@html content}