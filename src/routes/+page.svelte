<script lang="ts">
	import Row from './Row.svelte';

	let form = {
		site_plan_name: '',
		design_professional_name: '',
		design_professional_phone: '',
		tax_map: '',
		submission_date: '',
		submission_number: '',
		first_review: '',
		notes: ''
	};

	function printForm() {
		window.print();
	}

	function clearForm() {
		form = {
			site_plan_name: '',
			design_professional_name: '',
			design_professional_phone: '',
			tax_map: '',
			submission_date: '',
			submission_number: '',
			first_review: '',
			notes: ''
		};
	}

	function printAndClearForm() {
		printForm();
		clearForm();
	}
</script>

<h1>Review Checklist</h1>
<p>
	This checklist is to be completed by the design professional and submitted with the site plan.
</p>

<form>
	<table class="top_table">
		<tr>
			<td><label for="site_plan_name">Subdivision/Site Plan Name: </label></td>
			<td><input class="long_text" type="text" id="site_plan_name" name="site_plan_name" /></td>
		</tr>
		<tr>
			<td><label for="design_professional_name">Design Professional Name: </label></td>
			<td
				><input
					class="long_text"
					type="text"
					id="design_professional_name"
					name="design_professional_name"
				/></td
			>
		</tr>
		<tr>
			<td><label for="design_professional_phone">Design Professional Phone: </label></td>
			<td
				><input
					class="long_text"
					type="text"
					id="design_professional_phone"
					name="design_professional_phone"
				/></td
			>
		</tr>
		<tr>
			<td><label for="tax_map">Tax Map (PIN): </label></td>
			<td><input class="long_text" type="text" id="tax_map" name="tax_map" /></td>
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
		<Row />
	</table>
	<button type="button" on:click={printForm}>Print</button>
	<button type="button" on:click={clearForm}>Clear</button>
	<button type="button" on:click={printAndClearForm}>Print & Clear</button>
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
		color: #014b92;
	}

	h2 {
		color: #3a6eab;
		font-size: 1.5rem;
		margin-top: 2rem;
		margin-bottom: 0.5rem;
	}

	h3 {
		color: #3a6eab;
		font-size: 1.3rem;
		margin-top: 2rem;
		margin-bottom: 0.5rem;
	}
	.top_table td {
		padding-right: 2.5rem;
	}

	.long_text {
		width: 40rem;
	}

	.review_icons {
		width: 4rem;
		text-align: center;
	}

	.primary_table {
		margin-top: 2rem;
	}
</style>
