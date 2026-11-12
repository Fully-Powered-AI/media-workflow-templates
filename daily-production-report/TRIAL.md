# Daily production report: tried on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-10

The inputs were the invented example in [`example.md`](example.md): an invented ten-day short-film shoot, with people named by position and a letter. No client data was used.

**Inputs used:** the five inputs under "The inputs" in `public/example.md` (call sheet, timecard export, department reports, production notes, settings), followed with the fenced instruction block and the output format in `member/template.md`.

## An honest limit on this trial

The assistant that ran this trial printed the whole example file in one step, so it saw the example's published output before it produced its own. The output below was still worked out from the inputs and the template, and every total and check was recomputed by hand, but this is not a blind trial. The close match with the published example should be read with that in mind.

## What came out

```
DAILY PRODUCTION REPORT: Short film P, shoot day 6 of 10, Tuesday 3 March 2026

For: the production manager. Prepared from the call sheet (8 people), the timecard export (9 entries from 8 people), 4 department reports, the production notes and the settings.
Counts: 7 of the 8 people on the call sheet have a timecard. 1 person with a timecard is not on the call sheet. Queries: 5.

Day at a glance
Location: Location A (warehouse). General call: 07:00. Earliest logged call-in: 06:30 (Gaffer A, Production Assistant A).
Planned wrap: 18:00. Called wrap: 18:30. Latest logged wrap-out: 19:30 (Production Assistant A).
Call times: the logged call-in matches the call sheet for 7 of the 7 listed people who have a timecard. No differences.

Work planned and reported
Scene 14: done. Camera and Sound report it shot and recorded.
Scene 15: done. Camera reports one unreadable camera card and two takes shot again; Sound reports the wild track was not taken and asks for a pickup.
Scene 17: not started; moved to Wednesday 4 March (production notes). Grip and electric report the lighting rigged and left in place overnight; Art reports the dressing not finished and the door prop arriving tomorrow morning.

Department reports
Camera: scenes 14 and 15 shot, scene 17 not started, 22 setups, one camera card unreadable, two takes of scene 15 shot again.
Grip and electric: lighting for scene 17 rigged and left in place overnight; generator refuelled at 15:00.
Sound: scenes 14 and 15 recorded; wild track for scene 15 not taken; a pickup is requested.
Art: dressing for scene 17 not finished; the door prop arrives tomorrow morning.
Production: no report supplied.

Schedule changes
1. Scene 17 moved to Wednesday 4 March because the light went at 17:45 (production notes).
2. Wrap called at 18:30 against a planned 18:00, 0:30 later (production notes).
3. Logged wrap-outs later than the called wrap of 18:30: Gaffer A 19:00, Grip A 19:00, Production Assistant A 19:30.
4. Location A access closes at 20:00 tomorrow (production notes).

Hours as written
Camera: 2 people, 2 entries, 22:30.
Grip and electric: 2 people, 2 entries, 23:00.
Sound: 1 person, 1 entry, no hours written (see query 2).
Art: 1 person, 2 entries, 9:00 (see query 3).
Production: 2 people, 2 entries, 18:30.
Day total: 73:00, from 8 of the 9 entries. The Sound entry is listed under Queries.

Queries: 5
1. Missing timecard. Script Supervisor A (Production, script supervisor) is on the call sheet with a 07:00 call and has no timecard. Ask: Script Supervisor A or the production office.
2. Incomplete entry. Sound Mixer A (Sound): call-in 07:00 and meal 30 written; wrap-out and hours blank. Note: "left before wrap; to confirm". Left out of every total. Ask: Sound Mixer A.
3. Overlapping entries. Art Assistant A (Art): 07:00 to 13:00 (5:30 written) and 12:30 to 16:00 (3:30 written, note "second set"). They overlap from 12:30 to 13:00, 30 minutes. Both are totaled as written (9:00), so the total may count the overlap twice. Ask: the Art department head.
4. Hours differ from times. Focus Puller A (Camera): 07:00 to 18:30 is 11:30; less the written meal of 0:30 is 11:00; hours written 11:30. Difference 0:30, above the 0:15 tolerance. Totaled as written. Ask: Focus Puller A or the Camera department head.
5. Not on the call sheet. Driver A (Production, driver): 10:00 to 17:00, meal 30, 6:30 written; not on the call sheet and not mentioned in the production notes. Totaled as written. Ask: the production office.

Hours disputed in the notes: none noted. Entries whose hours match their times: 7 of 9 (1 differs, 1 cannot be checked).

Draft for the production manager's check. The hours are totaled as written. No pay rule, overtime, meal-penalty or guild computation has been applied, and nothing has been sent or submitted.
```

## What was observed

- **Every required part was produced.** All slots of the output format appear, in order, and the queries come in the fixed order.
- **Totals recomputed by hand and agree:** Camera 22:30, Grip and electric 23:00, Art 9:00, Production 18:30, day 73:00 from 8 of 9 entries. Seven entries match their own span less meal; one differs (Focus Puller A, 0:30); one cannot be checked (Sound Mixer A).
- **Nothing triggered a stop.** The headers matched, there was one date, and nobody asked for a pay rule, a filled-in time or a submission, so the refusal paths were not exercised.
- **Compared with the published example,** the content is the same: the same five queries, totals, counts and schedule items. The differences are in form and wording only. The example uses bold headings and bullets; this run followed the template's plain-text layout. The example writes the Day total's last sentence as "The Sound entry is not included"; this run wrote "The Sound entry is listed under Queries", following the template's own bracket. This run quotes the "second set" note and the Driver's meal in the queries; the example does not. This run labels scenes 14 and 15 "done"; the example says "shot".
- **No fact appears in either output that is not in the inputs.** The one thing worth a second look: "the production manager" is a role from the settings, not a name; both outputs use the role.
- **Where the instructions were ambiguous and a guess was needed:**
  1. Status words for planned work are "done / partly done / not started / moved to date". Scene 17 is both not started and moved. This run used "not started; moved to ...". Scene 15 was shot with retakes and a missing wild track; "done" was chosen over "partly done", with the gaps stated.
  2. The department-report count (4) excludes the department with "no report supplied". The template does not say whether that department counts. The example counts four.
  3. Step 7 asks for "any access or booking date the notes give for the next day". The notes give a closing time (20:00 tomorrow), not a date. It was listed as a schedule change; the template does not say where it belongs.
  4. The camera report of an unreadable card and the sound report of a missed wild track are not queries under any listed kind, and the "Other" kind says "cannot be reconciled". They were left as report lines, not queries. A user may expect a follow-up.
  5. The called wrap is reported both in the day at a glance and as schedule change 2. That duplicates itself by design, but the template does not say so.
  6. When an entry is left out of a total, the output format says entries left out "are listed under Queries"; the example's wording differs. The template and its example disagree slightly here.
  7. For a person with two entries, the call-time comparison uses only the first entry; the template does not say how to treat a second entry for the same person.
- **Smaller points:** the default tolerance is written `0:15 or [your tolerance]` in the template body, which reads as a placeholder; the Version notes still say "Not yet tried on its invented example", which this trial changes.

## Edits made after this run

These were made on 10 November 2026, after the run above, in response to an independent review. The run was not repeated, and the output and observations above are left as recorded. The edits:

- The default timecard export is now taken to be for the call sheet's date unless it carries a date column.
- The default tolerance is written "0:15", with the customization left to "What to customize". A decimal that is not a whole number of minutes is now left out of the totals and queried, not rounded.
- Ambiguities 1, 2, 3, 4 and 7 above are each settled with one line in the procedure and the instruction block. A scene reported moved is "moved to [date]"; a scene done with a stated gap is "partly done"; only supplied reports are counted; a next-day closing time is listed as a schedule change; a problem a department report states stays in its line; a person with two entries is compared on the earlier call-in.
- The department or position mismatch and the dispute or safety incident exceptions are named under "Other" in the instruction block, and the block now says the output format is pasted with it.
- The instruction block now also stops when the export's date differs from the call sheet, asks the assistant to confirm one production, one date and one shoot day, and defines an incomplete entry (blank call-in, wrap-out, hours or meal, or wrap-out earlier than call-in, which is not computed). The "Production schedule rebuild" pointer was removed from the template and its related list, because that workflow template is a manufacturing build schedule, not a shoot schedule. These edits were not run again.
- The published example now quotes the "second set" note in query 3, as this run did. The example still labels scene 15 "partly done" and scene 17 "moved to Wednesday 4 March" where this recorded run printed "done" and "not started; moved to"; the record above is left as it was run.
- The observation that the Version notes still said "Not yet tried on its invented example" is out of date: they now say it was tried.
- In the published example, the call-times line now ends "No differences.", the status words follow the output format (scene 14 "done", scene 15 "partly done", scene 17 "moved to Wednesday 4 March"), and the day-total line follows the template's wording. No fact in the example changed.
