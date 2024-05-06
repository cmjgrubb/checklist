<script lang="ts">
	import Row from './Row.svelte';

	function handle_submit(event: Event) {
		/*TO DO*/
	}
</script>

<h1>Review Checklist</h1>
<p>
	This checklist is to be completed by the design professional and submitted with the site plan.
</p>

<form on:submit|preventDefault={handle_submit}>
	<table class="top_table">
		<tr>
			<td><label for="site_plan_name">Subdivision/Site Plan Name: </label></td>
			<td><input type="text" id="site_plan_name" name="site_plan_name" /></td>
		</tr>
		<tr>
			<td><label for="design_professional_name">Design Professional Name: </label></td>
			<td><input type="text" id="design_professional_name" name="design_professional_name" /></td>
		</tr>
		<tr>
			<td><label for="design_professional_phone">Design Professional Phone: </label></td>
			<td><input type="text" id="design_professional_phone" name="design_professional_phone" /></td>
		</tr>
		<tr>
			<td><label for="tax_map">Tax Map (PIN): </label></td>
			<td><input type="text" id="tax_map" name="tax_map" /></td>
		</tr>
		<tr>
			<td><label for="submission_date">Submission Date: </label></td>
			<td><input type="date" id="submission_date" name="submission_date" /></td>
		</tr>
		<tr>
			<td><label for="submission_number">Submission Number: </label></td>
			<td><input type="text" id="submission_number" name="submission_number" /></td>
		</tr>
	</table>

	<h2>Requirements</h2>
	<h3>Review Key</h3>
	<table>
		<tr><td class="review_icons">✅</td><td>OK</td></tr>
		<tr><td class="review_icons">⚠️</td><td>Incomplete</td></tr>
		<tr><td class="review_icons">N</td><td>Not Applicable</td></tr>
		<tr><td class="review_icons">❌</td><td>Unacceptable</td></tr>
	</table>

	<table class="primary_table">
		<thead>
			<tr>
				<th class="primary_th">Description</th>
				<th class="secondary_th">Design<br />Professional</th>
				<th class="secondary_th">First<br />Review</th>
				<th class="primary_th">Notes</th>
			</tr>
		</thead>
		<tr>
			<td colspan="4" class="section_td">General</td>
		</tr>
		<Row />
	</table>
</form>

<style>
	:global(body) {
		font-family: Arial, sans-serif;
		font-size: 16px;
		margin: 1.5rem;
		padding: 0rem;
		line-height: 2;
	}

	h1 {
		font-size: 2rem;
	}

	h2 {
		color: #014b92;
		font-size: 1.5rem;
		margin-top: 2rem;
		margin-bottom: 0.5rem;
	}

	h3,
	th {
		color: #014b92;
		font-size: 1.2rem;
		margin-top: 2rem;
		margin-bottom: 1rem;
		text-align: left;
	}

	.top_table td {
		padding-right: 2.5rem;
	}

	.review_icons {
		width: 4rem;
		text-align: center;
	}

	.primary_table {
		margin-top: 2rem;
	}

	.secondary_th {
		line-height: 1rem;
		font-size: 0.8rem;
	}

	.section_td {
		background-color: #014b92;
		color: #c0da2f;
		text-align: center;
		font-size: 1.2rem;
	}

	.description_td {
		padding-right: 5rem;
	}

	.select_td {
		padding-right: 2.5rem;
	}

	.notes {
		width: 35rem;
	}

	.color_pallette {
		color: #014b92;
		color: #c0da2f;
		color: #3a6eab;
		color: #468fc6;
		color: #e6a837;
		color: #8c877e;
		color: #b5b0a7;
		color: #d2cdc4;
	}
</style>
