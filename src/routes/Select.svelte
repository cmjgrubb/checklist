<script>
	export let name = '';
	export let id = '';
</script>

<select {name} {id}>
	<option value=""></option>
	<option value="ok">✅</option>
	<option value="incomplete">⚠️</option>
	<option value="not_applicable">N</option>
	<option value="unacceptable">❌</option>
</select>
