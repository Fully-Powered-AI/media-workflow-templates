# Sponsor delivery record: tried once on its example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-10

The inputs were the invented example in [example.md](example.md): the settings, the placement list for Sponsor A's October 2026 run, the publication and broadcast log (23 rows), the metrics (3 rows), the invoice history (3 invoices) and the lead's notes (3). No client data was used. The assistant that ran the template did not write it. It followed the template's instruction block and output format on those inputs and built its own record before comparing. One slip: the command that opened the example file also displayed the first part of the published record, as far as part of placement P3. The assistant had not yet worked the inputs when it saw that, so the counts and statuses for P1 to P3 were not independent of it. P4, P5, the billing questions, the totals and the decisions were worked out from the inputs alone, and the reader should weigh the trial with that in mind.

## What came out

```
SPONSOR DELIVERY RECORD: Sponsor A, October 2026 sponsorship

For: the partnerships lead, with the finance lead. Run 2026-10-01 to 2026-10-31. Prepared 2026-11-10. Scope named by the partnerships lead on 2026-11-09.
Inputs: 5 placements, 23 log rows, 3 metric rows, 3 invoices, 3 notes. Currency US dollars.

At a glance: 5 placements named. Evidence matches: 1. Evidence short: 3. No record found: 1. Records matched to no placement: 1. Billing questions: 3.

Placement register
P1 Pre-roll read on Evening Roundup (podcast)
 Named: 8 episodes, 2026-10-01 to 2026-10-31, asset A-PR-01, fee 4,800.00.
 Counted: 7 of 8 (L01, L02, L03, L04, L05, L06, L07). L07 had no placement reference and was matched by its asset.
 Outside the window: none.
 Other asset: none.
 Status: Evidence short, 7 of 8.
 Metric: M1, total downloads, 31,400, podcast host export, 2026-10-01 to 2026-10-22, not comparable: metric differs. Named: downloads per episode in first 7 days, podcast host export.
 Invoices: INV-1, 4,800.00, paid.
 Lead's note: none.
 Fulfilment: for the partnerships lead to confirm.

P2 Banner in Weekly Digest (newsletter)
 Named: 4 issues, 2026-10-01 to 2026-10-31, asset A-NL-01, fee 2,400.00.
 Counted: 3 of 4 (L09, L10, L11).
 Outside the window: L12, 2026-11-03.
 Other asset: none.
 Status: Evidence short, 3 of 4.
 Metric: M2, unique opens, 5,820, newsletter platform, 2026-10-02 to 2026-10-16, comparable. Named: unique opens, newsletter platform.
 Invoices: INV-2, 2,600.00, issued.
 Lead's note: P2: Sponsor A agreed by email on 2026-10-19 that issue 43 would run on 2026-11-03.
 Fulfilment: for the partnerships lead to confirm.

P3 30-second spot in Radio Block
 Named: 10 airings, 2026-10-01 to 2026-10-31, asset A-RB-30A, fee 3,000.00.
 Counted: 9 of 10 (L13, L14, L15, L16, L17, L18, L19, L20, L21).
 Outside the window: none.
 Other asset: L22, A-RB-30B.
 Status: Evidence short, 9 of 10.
 Metric: no measure named. Named: none named, none named.
 Invoices: INV-3, 4,800.00, issued (covers P3 and P4).
 Lead's note: P3: The spot with asset A-RB-30B aired on 2026-10-26 after the radio team swapped the file. No approval from Sponsor A is on file.
 Fulfilment: for the partnerships lead to confirm.

P4 Homepage sponsor panel
 Named: 14 days, 2026-10-12 to 2026-10-25, asset A-HP-01, fee 1,800.00.
 Counted: 14 of 14 (L23).
 Outside the window: none.
 Other asset: none.
 Status: Evidence matches.
 Metric: M3, impressions, 148,200, ad server, 2026-10-12 to 2026-10-24, not comparable: period does not cover the counted rows (the period ends 2026-10-24; the counted row runs to 2026-10-25). Named: impressions, ad server.
 Invoices: INV-3, 4,800.00, issued (covers P3 and P4).
 Lead's note: none.
 Fulfilment: for the partnerships lead to confirm.

P5 Social posts on the Publisher's main account
 Named: 2 posts, 2026-10-01 to 2026-10-31, asset A-SO-01, fee 1,000.00.
 Counted: 0 of 2 (none).
 Outside the window: none.
 Other asset: none.
 Status: No record found.
 Metric: no figure supplied. Named: reach, platform insights.
 Invoices: none.
 Lead's note: none.
 Fulfilment: for the partnerships lead to confirm.

Records matched to no placement
L08, 2026-10-27, Evening Roundup, A-PR-02, Pre-roll read episode 108. No placement reference, and its asset belongs to no placement.

Metrics that cannot be compared: 2
M1, P1: metric differs.
M3, P4: period does not cover the counted rows.

Billing questions: 3
B1. INV-1: 4,800.00, paid, covers P1. P1 is Evidence short, 7 of 8. The invoice equals the fee of P1 (4,800.00). Question for finance.
B2. INV-2: 2,600.00, issued, covers P2. P2 is Evidence short, 3 of 4. The invoice is 200.00 more than the fee of P2 (2,400.00). Question for finance.
B3. INV-3: 4,800.00, issued, covers P3 and P4. P3 is Evidence short, 9 of 10. P4 is Evidence matches. The invoice equals the fees of P3 and P4 (3,000.00 + 1,800.00). Question for finance.
Not invoiced: P5, fee 1,000.00, No record found.
Totals: fees named 13,000.00; fees of invoiced placements 12,000.00; invoiced 12,200.00 (difference 200.00); fees not invoiced 1,000.00.

Make-goods already agreed (lead's notes): none. The run note reads: "No make-good has been agreed."

Decisions for the partnerships lead: 6
1. P1, 7 of 8 episodes counted; L08 (asset A-PR-02) is listed as matching no placement; M1 cannot be compared (total downloads, where downloads per episode in the first 7 days is named). Question: how is the shortfall, the unmatched record and the metric to be handled?
2. P2, 3 of 4 issues counted; L12 (2026-11-03) is outside the window, and your note records Sponsor A's email agreeing that date. The agreement changes no count here. Question: how is the shortfall to be handled?
3. P3, 9 of 10 airings counted; L22 (2026-10-26) used asset A-RB-30B, and your note says no approval from Sponsor A is on file. Question: how is the shortfall and the other asset to be handled?
4. P4, 14 of 14 days counted; M3 cannot be compared because its period ends 2026-10-24 and the counted row runs to 2026-10-25. Question: how is the metric to be handled?
5. P5, 0 of 2 posts, No record found, not invoiced. Question: how is the missing record to be handled?
6. Records matched to no placement: L08 (2026-10-27, Evening Roundup, A-PR-02, episode 108). Question: what is this record, and does it belong to a placement?

Decisions for finance: 3
1. B1, INV-1 paid, 4,800.00, covers P1 (Evidence short, 7 of 8). Question: how is the paid invoice to be treated?
2. B2, INV-2 issued, 2,600.00 against a fee of 2,400.00 (difference 200.00), covers P2 (Evidence short, 3 of 4). Question: how are the difference and the shortfall to be treated?
3. B3, INV-3 issued, 4,800.00, equal to the fees of P3 and P4, P3 Evidence short, 9 of 10. Question: how is the issued invoice to be treated?

Every count traces to the log rows, metric rows, invoices and notes supplied for October 2026 sponsorship. The register changes no records and sends nothing. Fulfilment, any make-good and billing are decided by people.
```

## What was observed

- Every part of the output format was produced, and no step needed a stop. All headers matched, no identifier repeated, every date was real, and the totals line added up (12,000.00 + 1,000.00 = 13,000.00).
- The counts, statuses, the outside-the-window and other-asset lists, the unmatched record, both incomparable metrics, the 200.00 invoice difference, the three billing questions and the totals agree with the published example. Counting the example's rows by hand gives the same figures. No placement was called fulfilled, delivered or complete.
- Differences from the published example are in wording only. The example's lead decisions suggest more: decision 2 asks whether the agreed date makes issue 43 count, decision 4 asks whether a full-period impressions figure is to be requested, and decision 5 asks whether the posts ran somewhere the log does not cover. This run asked only how each item is to be handled. The example's P1 decision also ties the unmatched L08 to P1, and the example's finance decisions say "after the partnerships lead's decision". Neither is in the template's steps. The example prints the metric value as "total downloads 31,400" and this run put commas between the fields. The example's finance decisions restate the facts less fully than this run's.
- Every fact in this run's output is in the inputs. In the published example, the question about posts "anywhere the log does not cover" and the link of L08 to P1 are reasonable inferences rather than facts in the inputs. They stay inside the template's rule against recommending, but only just.

### Ambiguities and guesses

- The "Finance contact" setting is used in the output header but is not in the template's list of settings (step 1 of Inputs). The assistant took it from the example's settings.
- The template does not say how to show a placement that has several supplied metrics. The format has one Metric line. The example has at most one metric per placement, so this was not tested.
- When a measure is named for no placement ("none named") and metrics are supplied for other placements, the template says to write "no measure named". It does not say whether the "Named:" part of the line is then printed. This run printed "none named, none named", which reads badly.
- "Metrics that cannot be compared" and the lead decisions: it is not stated whether a placement with "no figure supplied" (P5 here) counts as a metric that cannot be compared. This run did not count it. The instruction block's list of lead decisions (step 9) also omits "its records left out" that the main procedure includes. This run followed the procedure.
- "Make-goods already agreed": the run note says none has been agreed. The template does not say whether to print "none" with the note or only the note. This run copied the example's choice.
- "Fees of invoiced placements" against "invoiced (difference)": the template does not say which two figures the difference is between. This run took invoiced minus fees of invoiced placements.
- The order of the lead's decisions is not specified. This run used the placement order with the unmatched records last.
- A row spanning dates that only partly fall inside the window is not covered for episodes, issues, airings and posts. The example has none, so it was not tested. The "Counted" line has no slot for a note such as "matched by its asset". This run added a sentence after the list.
- The acceptance tests are marked as not run. This run exercised the main path but none of the stop cases (header mismatch, requests to count a gap or propose a make-good).

## After the trial

Nothing above this heading was changed after the run. The template was revised afterwards, on 10 November 2026, in response to this record: it now lists the finance contact among the settings; says how several metrics for one placement are shown; leaves out "Named:" when no measure is named; says "no figure supplied" is neither an incomparable metric nor a decision of its own; brings the instruction block into line with the procedure; names the two figures in the totals line difference; covers invoices that share a placement (instalments) and a row only partly inside the window; and gives the "matched by its asset" note a place in the Counted line. The example's totals line and three of its lead decisions were reworded to match. A later round, after an independent review, made small changes: the Invoices line and the make-goods line of the output format gained the slots the run had used ("(covers ...)" for an invoice listing several placements, and the run note); the metric rule says "not comparable: no counted rows" for a placement with no counted row; the instruction block gained the stops for a blank required value, an impossible date or window, and an invoice listing a placement not in the scope; the rule for counting days is stated once; and the example's lead decisions were made plainer (decision 1 no longer ties L08 to P1; the questions on P3, P4 and P5 ask only whether the placement is fulfilled or how the metric is handled), so the quotation of the example's decisions 2, 4 and 5 under What was observed no longer matches the example. The example's trace line was brought into line with the output format. None of this changed the run's recorded output or observations. The revised template has not been run again, so none of these revisions is tried.
