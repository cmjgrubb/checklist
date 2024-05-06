<script lang="ts">
	import { ROW_DATA } from './Data';
</script>

{#each ROW_DATA as data}
	{#if data.data_id === 'header_row'}
		<tr>
			<td colspan="4" class="section_td">{data.data_name}</td>
		</tr>
	{:else}
		<tr>
			<td class="description_td"> <label for={data.data_id}>{data.data_name}</label></td>
			<td class="select_td">
				<select name="design_professional" id={data.data_id}>
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id={data.data_id}>
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id={data.data_id} name="notes" /></td>
		</tr>
	{/if}
{/each}

<style>
	.description_td {
		padding-right: 5rem;
	}

	.select_td {
		padding-right: 2.5rem;
	}

	.notes {
		width: 35rem;
	}
</style>
