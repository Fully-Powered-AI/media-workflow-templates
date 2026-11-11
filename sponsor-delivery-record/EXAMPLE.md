# Sponsor delivery record: an invented example

*Illustrative example with invented data.* The publisher, the sponsor, the shows, the assets, the figures and every date below are invented. The Publisher produces a podcast, a newsletter, a radio block and a website. Sponsor A bought five placements for October 2026. The Publisher's partnerships lead runs the record and, with finance, decides. People are referred to by role.

The inputs come first, in full, so the template can be run on them. The record follows.

## The inputs

### 1. Settings (typed by the partnerships lead)

```
Sponsor: Sponsor A
Run: October 2026 sponsorship
Today: 2026-11-10
Currency: US dollars
Scope named by: the partnerships lead, on 2026-11-09
Finance contact: the finance lead
```

### 2. The placement list (typed by the partnerships lead from the signed scope)

```
placement_id,description,asset_ref,quantity,unit,window_from,window_to,agreed_measure,measure_source,fee
P1,Pre-roll read on Evening Roundup (podcast),A-PR-01,8,episodes,2026-10-01,2026-10-31,downloads per episode in first 7 days,podcast host export,4800.00
P2,Banner in Weekly Digest (newsletter),A-NL-01,4,issues,2026-10-01,2026-10-31,unique opens,newsletter platform,2400.00
P3,30-second spot in Radio Block,A-RB-30A,10,airings,2026-10-01,2026-10-31,none named,none named,3000.00
P4,Homepage sponsor panel,A-HP-01,14,days,2026-10-12,2026-10-25,impressions,ad server,1800.00
P5,Social posts on the Publisher's main account,A-SO-01,2,posts,2026-10-01,2026-10-31,reach,platform insights,1000.00
```

### 3. The publication and broadcast log

```
log_ref,date_from,date_to,channel,asset_ref,description,placement_ref
L01,2026-10-01,2026-10-01,Evening Roundup,A-PR-01,Pre-roll read episode 101,P1
L02,2026-10-06,2026-10-06,Evening Roundup,A-PR-01,Pre-roll read episode 102,P1
L03,2026-10-08,2026-10-08,Evening Roundup,A-PR-01,Pre-roll read episode 103,P1
L04,2026-10-13,2026-10-13,Evening Roundup,A-PR-01,Pre-roll read episode 104,P1
L05,2026-10-15,2026-10-15,Evening Roundup,A-PR-01,Pre-roll read episode 105,P1
L06,2026-10-20,2026-10-20,Evening Roundup,A-PR-01,Pre-roll read episode 106,P1
L07,2026-10-22,2026-10-22,Evening Roundup,A-PR-01,Pre-roll read episode 107,
L08,2026-10-27,2026-10-27,Evening Roundup,A-PR-02,Pre-roll read episode 108,
L09,2026-10-02,2026-10-02,Weekly Digest,A-NL-01,Banner issue 40,P2
L10,2026-10-09,2026-10-09,Weekly Digest,A-NL-01,Banner issue 41,P2
L11,2026-10-16,2026-10-16,Weekly Digest,A-NL-01,Banner issue 42,P2
L12,2026-11-03,2026-11-03,Weekly Digest,A-NL-01,Banner issue 43,P2
L13,2026-10-05,2026-10-05,Radio Block,A-RB-30A,Spot airing,P3
L14,2026-10-07,2026-10-07,Radio Block,A-RB-30A,Spot airing,P3
L15,2026-10-09,2026-10-09,Radio Block,A-RB-30A,Spot airing,P3
L16,2026-10-12,2026-10-12,Radio Block,A-RB-30A,Spot airing,P3
L17,2026-10-14,2026-10-14,Radio Block,A-RB-30A,Spot airing,P3
L18,2026-10-16,2026-10-16,Radio Block,A-RB-30A,Spot airing,P3
L19,2026-10-19,2026-10-19,Radio Block,A-RB-30A,Spot airing,P3
L20,2026-10-21,2026-10-21,Radio Block,A-RB-30A,Spot airing,P3
L21,2026-10-23,2026-10-23,Radio Block,A-RB-30A,Spot airing,P3
L22,2026-10-26,2026-10-26,Radio Block,A-RB-30B,Spot airing,P3
L23,2026-10-12,2026-10-25,Website homepage,A-HP-01,Sponsor panel live,P4
```

### 4. The metrics supplied

```
metric_ref,placement_ref,period_from,period_to,metric,value,source
M1,P1,2026-10-01,2026-10-22,total downloads,31400,podcast host export
M2,P2,2026-10-02,2026-10-16,unique opens,5820,newsletter platform
M3,P4,2026-10-12,2026-10-24,impressions,148200,ad server
```

### 5. The invoice history

```
invoice_no,date,amount,placement_ids,status
INV-1,2026-10-05,4800.00,P1,paid
INV-2,2026-10-31,2600.00,P2,issued
INV-3,2026-11-02,4800.00,P3;P4,issued
```

### 6. The lead's notes

```
P2: Sponsor A agreed by email on 2026-10-19 that issue 43 would run on 2026-11-03.
P3: The spot with asset A-RB-30B aired on 2026-10-26 after the radio team swapped the file. No approval from Sponsor A is on file.
Run: No make-good has been agreed.
```

## The record

```
SPONSOR DELIVERY RECORD: Sponsor A, October 2026 sponsorship

For: the partnerships lead, with the finance lead. Run 2026-10-01 to 2026-10-31. Prepared 2026-11-10. Scope named by the partnerships lead on 2026-11-09.
Inputs: 5 placements, 23 log rows, 3 metric rows, 3 invoices, 3 notes. Currency US dollars.

At a glance: 5 placements named. Evidence matches: 1. Evidence short: 3. No record found: 1. Records matched to no placement: 1. Billing questions: 3.

Placement register
P1 Pre-roll read on Evening Roundup (podcast)
 Named: 8 episodes, 2026-10-01 to 2026-10-31, asset A-PR-01, fee 4,800.00.
 Counted: 7 of 8 (L01, L02, L03, L04, L05, L06, L07). L07 has no placement reference and was matched by its asset.
 Outside the window: none.
 Other asset: none.
 Status: Evidence short, 7 of 8.
 Metric: M1, total downloads 31,400, podcast host export, 2026-10-01 to 2026-10-22, not comparable: metric differs. Named: downloads per episode in first 7 days, podcast host export.
 Invoices: INV-1, 4,800.00, paid.
 Lead's note: none.
 Fulfilment: for the partnerships lead to confirm.

P2 Banner in Weekly Digest (newsletter)
 Named: 4 issues, 2026-10-01 to 2026-10-31, asset A-NL-01, fee 2,400.00.
 Counted: 3 of 4 (L09, L10, L11).
 Outside the window: L12, 2026-11-03.
 Other asset: none.
 Status: Evidence short, 3 of 4.
 Metric: M2, unique opens 5,820, newsletter platform, 2026-10-02 to 2026-10-16, comparable. Named: unique opens, newsletter platform.
 Invoices: INV-2, 2,600.00, issued.
 Lead's note: Sponsor A agreed by email on 2026-10-19 that issue 43 would run on 2026-11-03.
 Fulfilment: for the partnerships lead to confirm.

P3 30-second spot in Radio Block
 Named: 10 airings, 2026-10-01 to 2026-10-31, asset A-RB-30A, fee 3,000.00.
 Counted: 9 of 10 (L13, L14, L15, L16, L17, L18, L19, L20, L21).
 Outside the window: none.
 Other asset: L22, A-RB-30B.
 Status: Evidence short, 9 of 10.
 Metric: no measure named.
 Invoices: INV-3, 4,800.00, issued (covers P3 and P4).
 Lead's note: The spot with asset A-RB-30B aired on 2026-10-26 after the radio team swapped the file. No approval from Sponsor A is on file.
 Fulfilment: for the partnerships lead to confirm.

P4 Homepage sponsor panel
 Named: 14 days, 2026-10-12 to 2026-10-25, asset A-HP-01, fee 1,800.00.
 Counted: 14 of 14 (L23).
 Outside the window: none.
 Other asset: none.
 Status: Evidence matches.
 Metric: M3, impressions 148,200, ad server, 2026-10-12 to 2026-10-24, not comparable: period does not cover the counted rows (the period ends 2026-10-24; the counted rows run to 2026-10-25). Named: impressions, ad server.
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
L08, 2026-10-27, Evening Roundup, A-PR-02, Pre-roll read episode 108. No placement reference; its asset belongs to no placement.

Metrics that cannot be compared: 2
M1 (P1): metric differs.
M3 (P4): period does not cover the counted rows.

Billing questions: 3
B1. INV-1: 4,800.00, paid, covers P1. P1 is Evidence short, 7 of 8. The invoice equals the fee of P1 (4,800.00). Question for finance: how is the paid invoice to be treated while P1 is short?
B2. INV-2: 2,600.00, issued, covers P2. P2 is Evidence short, 3 of 4. The invoice is 200.00 more than the fee of P2 (2,400.00). Question for finance: how are the shortfall and the 200.00 difference to be treated?
B3. INV-3: 4,800.00, issued, covers P3 and P4. P3 is Evidence short, 9 of 10, with one airing under another asset. P4 is Evidence matches. The invoice equals the fees of P3 and P4 (3,000.00 + 1,800.00). Question for finance: how is the issued invoice to be treated while P3 is short?
Not invoiced: P5, fee 1,000.00, No record found.
Totals: fees named 13,000.00; fees of invoiced placements 12,000.00; invoiced 12,200.00 (difference 200.00, invoiced minus fees of invoiced placements); fees not invoiced 1,000.00.

Make-goods already agreed (lead's notes): none. The run note reads: "No make-good has been agreed."

Decisions for the partnerships lead: 6
1. P1, 7 of 8 episodes counted. M1 cannot be compared with the named measure: it is total downloads, where the named measure is downloads per episode in first 7 days. Question: is P1 fulfilled, and how are the shortfall and the metric to be handled?
2. P2, 3 of 4 issues counted. Issue 43 (L12) ran on 2026-11-03, outside the window; your note records Sponsor A's email agreeing that date. Nothing in the register counts it. Question: does the agreed date make issue 43 count for P2?
3. P3, 9 of 10 airings counted. One airing (L22, 2026-10-26) used asset A-RB-30B; your note says no approval from Sponsor A is on file. Question: is P3 fulfilled?
4. P4, 14 of 14 days counted. M3 cannot be compared with the named measure: its period ends 2026-10-24 and the counted rows run to 2026-10-25. Question: how is the metric to be handled?
5. P5, no record found, nothing invoiced. No log row matches P5. Question: is P5 fulfilled?
6. L08 (2026-10-27, Evening Roundup, asset A-PR-02) matches no placement. Question: what is this record?

Decisions for finance: 3
1. B1, INV-1, paid, P1 Evidence short (7 of 8): the facts as above. Question: how is the paid invoice to be treated, after the partnerships lead's decision on P1?
2. B2, INV-2, issued, P2 Evidence short (3 of 4), 200.00 above the fee: the facts as above. Question: how are the shortfall and the 200.00 difference to be treated, after the partnerships lead's decision on P2?
3. B3, INV-3, issued, P3 Evidence short (9 of 10), P4 Evidence matches: the facts as above. Question: how is the issued invoice to be treated, after the partnerships lead's decision on P3?

Every count traces to the log rows, metric rows, invoices and notes supplied for October 2026 sponsorship. The register changes no records and sends nothing. Fulfilment, any make-good and billing are decided by people.
```
