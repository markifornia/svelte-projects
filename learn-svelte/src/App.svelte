<script>
	let editor = $state.raw({
		theme: 'dark',
		content: '<h1>Svelte</h1>'
	})
</script>

<textarea class="editor" value={editor.content} oninput={e => editor.content = e.target.value} spellcheck="false"></textarea>

{@html editor.content}