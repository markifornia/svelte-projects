<script>
	let editor = $state({
		theme: 'dark',
		content: '<h1>Svelte</h1>'
	})

	function saveEditorState() {
		const editorState = structuredClone($state.snapshot(editor))
		console.log(editorState);
	}

	saveEditorState();
</script>

<textarea
	class="editor"
	value={editor.content}
	oninput={(e) => {
		editor = {
			...editor,
			content: e.target.value
		}
	}}
	spellcheck="false"
></textarea>

{@html editor.content}