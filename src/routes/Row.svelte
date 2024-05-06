<script lang="ts">
	import { ROW_DATA } from './Data';
</script>

{#each ROW_DATA as data}
	{#if data.data_id === 'header_row'}
		<tr>
			<td colspan="4" class="section_td">{data.data_name}</td>
		</tr>
		<tr>
			<th class="primary_th">Description</th>
			<th class="secondary_th">Design<br />Professional</th>
			<th class="secondary_th">First<br />Review</th>
			<th class="primary_th">Notes</th>
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
			<td><textarea class="notes" id={data.data_id} name="notes" rows="3" /></td>
		</tr>
	{/if}
{/each}

<style>
	.section_td {
		color: #3a6eab;
		font-size: 1.5rem;
		padding-top: 2rem;
		padding-bottom: 1rem;
	}

	.description_td {
		padding-right: 5rem;
	}

	.select_td {
		padding-right: 2.5rem;
	}

	.notes {
		width: 35rem;
		height: 3rem;
		margin-top: 1rem;
	}

	.primary_th {
		color: #3a6eab;
		font-size: 1.2rem;
		margin-top: 2rem;
		margin-bottom: 1rem;
		text-align: left;
	}

	.secondary_th {
		color: #3a6eab;
		line-height: 1rem;
		font-size: 0.8rem;
		text-align: left;
	}
</style>
