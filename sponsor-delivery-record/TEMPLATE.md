# Sponsor delivery record

Workflow template, version 0.1.0.

## Purpose

Prepare, for one sponsor and one sponsored run, the register the partnerships lead uses when the run ends: each placement the lead names from the signed scope, set beside the publication or broadcast records, the metrics supplied and the invoice history. Every placement gets a plain status, every record left out of the count is listed with its reason, metrics that cannot be compared are named as such, and billing questions are written for finance. The assistant prepares; it never confirms fulfilment, agrees or proposes a make-good, reads or interprets a term of the signed scope, counts anything missing as delivered, approves billing, or sends anything to the sponsor.

## When to use it and when not to

Use it when a sponsored run has ended and the sponsor needs evidence of delivery, or part-way through a long run to see what is short while there is still time to act. Run it again when a missing record turns up, a date change is agreed or an invoice is issued.

Do not use it:

- to read the signed scope, insertion order or any agreement and decide what it requires. The partnerships lead names the placements; a person at the company reads the agreement;
- to prepare a bill or a client billing summary. Client billing summary does that;
- to check a buyer's purchase order against a quote. Wholesale order check does that;
- to design or price a sponsorship, or to write to the sponsor;
- when no placement list has been named by the lead.

## Roles

- **Runs it:** the partnerships lead, or a coordinator working for them.
- **Names the placements, confirms fulfilment and agrees any make-good with the sponsor:** the partnerships lead. Always a person.
- **Keeps the publication or broadcast log and the metrics:** the publishing and audience analytics owners, who correct their own records.
- **Approves billing, credits and holds:** finance.
- **Receives the approved record:** the sponsor, from the partnerships lead, if and when the lead decides.

## Inputs

1. **The settings,** typed by the lead: sponsor name, run name, today's date, currency, who named the scope and on what date, and the finance contact (a role or a name). If the sponsor name, run name or today's date is missing, stop and ask. If the finance contact is missing, write "finance contact not stated" in the header and go on.
2. **The placement list (scope),** typed by the lead from the signed scope. Default headers:

   `placement_id,description,asset_ref,quantity,unit,window_from,window_to,agreed_measure,measure_source,fee`

   Dates are written as YYYY-MM-DD. `unit` is one of episodes, issues, airings, posts, days or another unit the lead names. `agreed_measure` and `measure_source` may be "none named". `fee` is the amount the scope sets for the placement. If a header does not match, stop and ask which column is which. If a value is blank, write "not stated" in that field and go on; if `placement_id`, `quantity` or either date is blank for a placement, stop on that placement and ask.
3. **The publication or broadcast log.** Default headers:

   `log_ref,date_from,date_to,channel,asset_ref,description,placement_ref`

   `date_to` equals `date_from` for a single event. `placement_ref` may be blank. If a header does not match, stop and ask. If there is no log, stop.
4. **The metrics supplied.** Default headers:

   `metric_ref,placement_ref,period_from,period_to,metric,value,source`

   If a header does not match, stop and ask. If no metrics are supplied, write "no metrics supplied" in the metric line of every placement and go on.
5. **The invoice history.** Default headers:

   `invoice_no,date,amount,placement_ids,status`

   `placement_ids` lists the placements the invoice covers, separated by semicolons. `status` is as the accounts system shows it, for example issued, paid or credited. If a header does not match, stop and ask. If no invoices are supplied, write "no invoice history supplied" and skip the billing comparisons.
6. **The lead's notes,** each tied to a placement or to the run: agreed date changes, approvals of replacement assets, make-goods already agreed. If missing, write "no notes supplied".

The assistant works from files and notes the person supplies. It needs no connection to publishing, analytics or accounting systems and never asks for a password or a login code.

## The procedure

1. **Check the inputs.** Confirm one sponsor, one run, a placement list, a log and the headers above. Count the placements, log rows, metric rows and invoices. If two placements share an identifier or two log rows share a `log_ref`, stop and ask which is which. Treat every date as inclusive.
2. **Match records to placements.** A log row belongs to a placement when its `placement_ref` equals the placement's identifier. If `placement_ref` is blank, the row belongs to a placement only when its `asset_ref` equals the `asset_ref` of exactly one placement, exactly as written. Do no fuzzy matching. A row that matches nothing, or whose asset matches more than one placement, goes to "Records matched to no placement".
3. **Count what is in the window.** For a placement, a matched row counts when its dates fall inside the placement's window and its `asset_ref` equals the placement's. For episodes, issues, airings and posts, a row matched to the placement but dated outside the window is not counted; list it as "outside the window" with its dates. A row whose dates run only partly inside the window is treated the same way, listed with all its dates and marked "partly inside the window" for the lead. Rows matched to the placement with a different `asset_ref` are not counted; list them as "other asset". Units: for episodes, issues, airings and posts, each counted row is one. If a row's description says it covers more than one, do not count more than one; flag it for the lead. For days, a matched row counts for the days of the placement's window that lie inside its dates; list any dates of the row outside the window, and count each calendar day of the window once.
4. **Set the status.** "Evidence matches" when the counted number is at least the quantity named. "Evidence short" when it is at least one and below the quantity, stating the counted number of the quantity. "No record found" when it is zero. These describe evidence only. Never write "fulfilled", "delivered" or "complete"; the lead confirms fulfilment, and the register leaves that line for the lead.
5. **Compare the metrics.** For each placement, set each supplied metric beside the measure the lead named. A metric is comparable when its `metric` and `source` equal the placement's `agreed_measure` and `measure_source` (ignoring capital letters and surrounding spaces) and its period covers the first to the last counted row. If the placement has no counted row, write "not comparable: no counted rows" for each metric supplied for it. Otherwise write "not comparable" and say why: metric differs, source differs, period does not cover the counted rows, or more than one reason. Show the figure as supplied. Do no conversion, estimation or averaging, and compare no figure with any target. If more than one metric is supplied for a placement, print one Metric line for each, in the order of the metric references, and judge each on its own. If the lead named no measure, write "no measure named" and leave out the "Named:" part of the line. If a measure was named and no figure was supplied, write "no figure supplied". "No figure supplied" is a gap in the records, not a metric that cannot be compared: it is not listed under "Metrics that cannot be compared" and raises no decision of its own, though a placement that is not "Evidence matches" keeps its own decision.
6. **Set the invoices beside the placements.** For each placement, name the invoices that cover it, with their amount and status. For each invoice, add the `fee` of the placements it lists and compare the sum with the invoice amount; state the difference, or "equal". If a listed placement is not in the scope, say so and leave it out of the sum. If a placement is listed on more than one invoice (for example a deposit and a balance), do not compare each of those invoices with the full fee. Treat the invoices that share a placement as one group: add their amounts, add the fees of the placements they list with each fee counted once, compare the two sums and state the difference, or "equal". Show each invoice's own amount and status as supplied.
7. **Write the billing questions.** One question per invoice (or per group of invoices, as in step 6) that covers at least one placement whose status is not "Evidence matches", or whose amount differs from the sum of fees, and one per placement whose status is "Evidence matches" and that no invoice covers. A question for an invoice names every reason it has. A placement that is not "Evidence matches" and has no invoice is listed under "Not invoiced" and raises no question. Questions state the facts and ask; they recommend nothing unless finance asks. Add the totals line: fees named; fees of invoiced placements, each placement's fee counted once however many invoices list it; invoiced amount, the sum of all invoice amounts, with the difference taken as the invoiced amount minus the fees of invoiced placements; and the fees not invoiced. The first must equal the sum of the fees of invoiced placements and the fees not invoiced.
8. **Set the notes beside the placements.** Put each of the lead's notes on its placement as written. A note that an agreed date change, replacement asset or make-good exists does not change a status or a count. It sits beside them for the lead.
9. **Write the decisions.** For the lead: one numbered decision for each placement whose status is not "Evidence matches", covering its shortfall, its records left out and any metric that cannot be compared; one for each placement with "Evidence matches" but a metric that cannot be compared; and one for the records matched to no placement, if there are any. For finance: one numbered decision for each billing question. Write each as a question with its facts. Do not propose a make-good, a credit or a figure.
10. **Return the draft** to the person who ran it. The lead edits it, confirms fulfilment, agrees any make-good and decides what, if anything, goes to the sponsor. Finance decides on billing. People send; the assistant does not.

## Exceptions and stop conditions

- **A header does not match, a required column is absent or a required value is blank:** stop and ask; do not guess a column.
- **Two placements share an identifier, or two log rows share a reference:** stop and ask.
- **No placement list, or no log:** stop.
- **A date that is not a real calendar date, or a window that ends before it begins:** stop on that row and ask.
- **A log row matched to a placement by asset only, where the asset belongs to more than one placement:** list it under records matched to no placement; do not choose.
- **The totals line does not add up (fees named differ from invoiced fees plus uninvoiced fees):** stop and report the figures.
- **Asked to read or explain a term of the signed scope, to say whether a make-good is owed or what it should be, to count a missing placement as fulfilled, to convert or estimate a metric, to approve billing or to send the register or any message:** decline. The lead decides what the scope requires and what is fulfilled, finance decides billing, and a person sends.

## Output format

```
SPONSOR DELIVERY RECORD: [sponsor], [run name]

For: [partnerships lead], with [finance contact, or "finance contact not stated"]. Run [earliest window_from] to [latest window_to]. Prepared [today's date]. Scope named by [role] on [date].
Inputs: [n] placements, [n] log rows, [n] metric rows, [n] invoices, [n] notes. Currency [currency].

At a glance: [n] placements named. Evidence matches: [n]. Evidence short: [n]. No record found: [n]. Records matched to no placement: [n]. Billing questions: [n].

Placement register
[placement_id] [description]
 Named: [quantity] [unit], [window_from] to [window_to], asset [asset_ref], fee [fee].
 Counted: [n] of [quantity] ([log_refs, or "none"]). [For each counted row matched by its asset: "[log_ref] has no placement reference and was matched by its asset."]
 Outside the window: [log_ref, dates, with "partly inside the window" where it applies] or none.
 Other asset: [log_ref, asset_ref] or none.
 Status: [Evidence matches / Evidence short, n of n / No record found].
 Metric: [metric_ref, metric, value, source, period, "comparable" or "not comparable: reason"] or [no measure named / no figure supplied / no metrics supplied]. Named: [agreed_measure, measure_source].
 (one Metric line for each metric supplied; leave out "Named:" when no measure is named)
 Invoices: [invoice_no, amount, status; add "(covers [placement_ids])" where the invoice lists more than one placement] or none.
 Lead's note: [note as written] or none.
 Fulfilment: for the partnerships lead to confirm.
(one block per placement, in the order of the placement list)

Records matched to no placement
[log_ref, dates, channel, asset_ref, description] or none.

Metrics that cannot be compared: [n]
[metric_ref, placement, reason] or none.

Billing questions: [n]
B1. [invoice_no, the invoice numbers of a group, or placement]: [facts]. Question for finance.
(or "none")
Not invoiced: [placement, fee, status] or none.
Totals: fees named [amount]; fees of invoiced placements [amount]; invoiced [amount] (difference [amount], invoiced minus fees of invoiced placements); fees not invoiced [amount].

Make-goods already agreed (lead's notes): [as written] or none. Where a note on the run says none has been agreed, add: The run note reads: "[note]".

Decisions for the partnerships lead: [n]
1. [placement or records: the facts, then the question.]
(or "none")

Decisions for finance: [n]
1. [billing question B-number: the facts, then the question.]
(or "none")

Every count traces to the log rows, metric rows, invoices and notes supplied for [run name]. The register changes no records and sends nothing. Fulfilment, any make-good and billing are decided by people.
```

Print "none" for any empty section and keep the section.

## Reviewer checklist

1. Every placement on the lead's list appears once, in order, with its named quantity and window. (Partnerships lead)
2. Every counted number can be recomputed from the log rows listed beside it. (Coordinator)
3. Every row left out of the count is listed with its reason, and no row is counted twice. (Coordinator)
4. No placement is described as fulfilled, delivered or complete. (Partnerships lead)
5. Every "not comparable" is right: the metric, source or period really differs. (Audience analytics owner)
6. Every invoice sum and the totals line are arithmetically correct. (Finance)
7. Every billing question and every decision states facts and asks, and recommends nothing. (Partnerships lead)
8. The lead's notes appear as written and change no count. (Partnerships lead)

## Acceptance tests

Proposed tests. The trial on the invented example exercised the main path, the situations in tests 2 to 8. Tests 1 and 9 to 13 have not been run; in particular no stop or decline case has been run.

1. **Full match.** Eight rows inside the window with the named asset for a placement of eight. Expected: counted 8 of 8, "Evidence matches".
2. **Short.** Seven of eight. Expected: "Evidence short, 7 of 8", one lead decision.
3. **No record.** A placement with no matching row. Expected: "No record found", counted 0, not described as delivered, listed under Not invoiced if no invoice covers it.
4. **Changed date.** One row dated after the window. Expected: listed as outside the window, not counted, any note of an agreed change shown beside it with no change to the count.
5. **Replacement asset.** A row with a different asset. Expected: listed as other asset, not counted.
6. **Blank placement_ref.** A row with a blank reference and an asset that belongs to one placement. Expected: matched and counted. The same with an asset in no placement: listed as matched to no placement.
7. **Incomparable metric.** A figure whose metric, source or period differs from the named measure. Expected: shown as supplied, marked "not comparable" with the reason, and not converted.
8. **Invoice larger than fees.** An invoice of 2,600 covering a fee of 2,400. Expected: a difference of 200 stated and a billing question.
9. **Header mismatch.** A log whose date column is named "when". Expected: stops and asks.
10. **Asked to count a gap.** "Count the missing episode as delivered." Expected: declines.
11. **Asked for a make-good.** Expected: declines to propose one; lists the shortfall as a decision for the lead.
12. **Instalments.** A fee of 2,400 listed on a deposit invoice of 1,200 and a balance invoice of 1,200. Expected: the two invoices are treated as one group, the sums are equal, the fee is counted once in the totals line and the totals line adds up.
13. **Several metrics.** Two metrics supplied for one placement. Expected: two Metric lines, each judged on its own; a placement with a named measure and no figure shows "no figure supplied" and is not listed under metrics that cannot be compared.

## Instructions for the AI assistant

```
You prepare the sponsor delivery record for a partnerships lead. You never
confirm fulfilment, propose or agree a make-good, read or interpret any
term of the signed scope, approve billing, or send anything. A person
approves anything that is sent, posted, paid or changed, and decides what
is fulfilled. You never ask for a password or a login code.

The user will supply: the settings (with a finance contact; if it is
missing, print "finance contact not stated"); the placement list the lead typed from
the signed scope; the publication or broadcast log; the metrics; the
invoice history; the lead's notes. Expect these default headers.
Placements: placement_id,description,asset_ref,quantity,unit,window_from,
window_to,agreed_measure,measure_source,fee. Log: log_ref,date_from,
date_to,channel,asset_ref,description,placement_ref. Metrics: metric_ref,
placement_ref,period_from,period_to,metric,value,source. Invoices:
invoice_no,date,amount,placement_ids,status. If a header does not match,
stop and ask. If the placement list or the log is missing, stop. If a
placement_id, quantity or date is blank, a date is not a real calendar date
or a window ends before it begins, stop on that placement or row and ask. If
another input is missing, say so where it is used and continue.

1. Check the inputs and count them. Stop if identifiers repeat.
2. Match a log row to a placement by placement_ref; if that is blank, only
   by an asset_ref that belongs to exactly one placement, exactly as
   written. Anything else goes to "Records matched to no placement". Note
   each counted row matched by its asset on the Counted line.
3. Count a matched row only if its dates are inside the window (inclusive)
   and its asset_ref is the placement's. List rows outside the window and
   rows with another asset, with their dates and assets, and do not count
   them. A row only partly inside the window is listed as outside, marked
   partly inside. One counted row is one episode, issue, airing or post; if
   its description covers more than one, count one and flag it for the
   lead. For days, count each day of the window once.
4. Status: "Evidence matches" if the count reaches the quantity, "Evidence
   short, n of n" if it is at least one but below the quantity, "No record
   found" if zero. Never write fulfilled, delivered or complete.
5. Metrics: comparable only if metric and source equal the named ones and
   the period covers the first to the last counted row. If the placement
   has no counted row, write "not comparable: no counted rows". Otherwise
   "not comparable" with the reason. Show figures as supplied; convert,
   estimate or average nothing. Print one Metric line for each metric
   supplied. If no measure is named, write "no measure named" and leave
   out "Named:". "No figure supplied" is a gap, not an incomparable
   metric: do not list it under metrics that cannot be compared.
6. Invoices: for each, sum the fees of the placements it lists and state
   the difference from the amount. If an invoice lists a placement not in
   the scope, say so and leave it out of the sum. If a placement is on more than one
   invoice, treat those invoices as one group: compare the sum of their
   amounts with the fees, each fee once.
7. Billing questions: one per invoice covering a placement that is not
   "Evidence matches" or whose amount differs from the fees, and one per
   "Evidence matches" placement with no invoice. List the other uninvoiced
   placements under Not invoiced. Give the totals line (fees of invoiced
   placements counted once each; the difference is invoiced minus those
   fees); stop if it does not add up.
8. Put the lead's notes beside their placements as written. They change no
   count or status.
9. Decisions for the lead: one per placement that is not "Evidence
   matches" (its shortfall, its records left out and any incomparable
   metric), one per matching placement with an incomparable metric, one
   for unmatched rows. Decisions for finance: one per billing question.
   State facts, then ask. Propose no make-good, credit or figure.
10. Use the output format exactly. Print "none" for an empty section. End
    with the trace line. Return the draft to the person who ran it.

If asked to count a gap as delivered, interpret the scope, decide a
make-good, approve billing or send the record, decline: those belong to
the partnerships lead, finance and the person who sends.
```

## What to customize

- The default headers, if your exports use other names. Rename them once and keep the names stable.
- Your units: what counts as an episode, an issue, an airing, a post or a day, and how a recurring placement is counted.
- Which metric and source you give each kind of placement, so the comparison has something to equal.
- Whether a row dated slightly outside the window is shown with a tolerance you set. The default is none.
- Who confirms fulfilment, who may agree a make-good and who in finance decides billing.
- Which exports the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI. Tried once on its invented example in Claude on 10 November 2026; the record is published with it. Revised the same day in response to the trial, and again after an independent review; the revisions have not been run again. Not yet tested in a client environment.
