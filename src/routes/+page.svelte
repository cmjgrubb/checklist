<script lang="ts">
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
		<tr>
			<td class="description_td">
				<label for="owner_contact_info"
					>Owner's/developer's contact information, including Email</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="owner_contact_info">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="owner_contact_info">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="owner_contact_info" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="magesterial_district"
					>Magesterial district, tax map, and address, if applicable</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="magesterial_district">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="magesterial_district">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="magesterial_district" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="utility_contact">Utility contact information</label></td
			>
			<td class="select_td">
				<select name="design_professional" id="utility_contact">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="utility_contact">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="utility_contact" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="north_arrow">North arrow on all plan sheets</label></td
			>
			<td class="select_td">
				<select name="design_professional" id="north_arrow">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="north_arrow">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="north_arrow" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="scale_references">Scale references on all plan sheets</label></td
			>
			<td class="select_td">
				<select name="design_professional" id="scale_references">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="scale_references">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="scale_references" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="spec_compliance"
					>Current FW Standards and Specifications have been reviewed for compliance at <a
						href="https://frederickwater.com"
						target="_blank">frederickwater.com</a
					></label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="spec_compliance">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="spec_compliance">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="spec_compliance" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="fw_notes">Current FW construction notes are on plans</label></td
			>
			<td class="select_td">
				<select name="design_professional" id="fw_notes">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="fw_notes">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="fw_notes" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="easements"
					>All existing easements are shown including deed book & page or instrument number</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="easements">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="easements">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="easements" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="vicinity_map">Vicinity map</label></td>
			<td class="select_td">
				<select name="design_professional" id="vicinity_map">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="vicinity_map">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="vicinity_map" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="general_layout">General layout sheet</label></td>
			<td class="select_td">
				<select name="design_professional" id="general_layout">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="general_layout">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="general_layout" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="infrastructure_shown"
					>Current existing water and sanitary sewer infrastructure is shown and described</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="infrastructure_shown">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="infrastructure_shown">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="infrastructure_shown" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="onsite_fw_easements">Required onsite FW easements are identified</label></td
			>
			<td class="select_td">
				<select name="design_professional" id="onsite_fw_easements">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="onsite_fw_easements">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="onsite_fw_easements" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="offsite_fw_easements">Required off site FW easements are identified</label></td
			>
			<td class="select_td">
				<select name="design_professional" id="offsite_fw_easements">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="offsite_fw_easements">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="offsite_fw_easements" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="no_trees_shrubs"
					>Note has been added to landscape drawings that no trees or shrubs shall be placed on FW
					easements</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="no_trees_shrubs">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="no_trees_shrubs">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="no_trees_shrubs" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="fw_standards_project_phase"
					>Project Acceptance Requirements per FW standards (page 4) have been considered in project
					phasing</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="fw_standards_project_phase">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="fw_standards_project_phase">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="fw_standards_project_phase" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="exiting_site_conditions"
					>Existing site conditions are shown and labeled ie. ex. structures, utilities, etc.</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="exiting_site_conditions">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="exiting_site_conditions">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="exiting_site_conditions" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="mdp"
					>Master development plan reviewed for compliance and MDP #, date included. Any variance
					from MDP water or sewer requirements is explained</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="mdp">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="mdp">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="mdp" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="proffer_statement"
					>Proffer statement reviewed for compliance and copy included</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="proffer_statement">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="proffer_statement">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="proffer_statement" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="exceptions_to_requirements">Exceptions to FW requirements are described</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="exceptions_to_requirements">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="exceptions_to_requirements">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="exceptions_to_requirements" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="lines_minimized"
					>Length of water and sewer lines on private property to be owned by FW kept to minimum</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="lines_minimized">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="lines_minimized">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="lines_minimized" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="lot_building_street"
					>Lot numbers, building numbers and street names are shown on all sheets</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="lot_building_street">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="lot_building_street">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="lot_building_street" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="reconciled"
					>All plan sheets have been reconciled to reflect the same information</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="reconciled">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="reconciled">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="reconciled" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="field_adjustment"
					>Existing FW infrastructure requiring field adjustment where grade changes occur has been
					shown</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="field_adjustment">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="field_adjustment">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="field_adjustment" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td">
				<label for="abandoned"
					>Existing FW facilities to be removed or abandoned are noted accordingly. Significant
					items, fire hydrants, valves, etc., are noted to be furnished to FW inspector</label
				></td
			>
			<td class="select_td">
				<select name="design_professional" id="abandoned">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="abandoned">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="abandoned" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
		<tr>
			<td class="description_td"> <label for="//TODO">//TODO</label></td>
			<td class="select_td">
				<select name="design_professional" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select></td
			>
			<td class="select_td">
				<select name="first_review" id="//TODO">
					<option value=""></option>
					<option value="ok">✅</option>
					<option value="incomplete">⚠️</option>
					<option value="not_applicable">N</option>
					<option value="unacceptable">❌</option>
				</select>
			</td>
			<td><input class="notes" type="text" id="//TODO" name="notes" /></td>
		</tr>
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
