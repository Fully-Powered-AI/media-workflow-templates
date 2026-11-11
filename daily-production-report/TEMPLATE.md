# Daily production report

Capability template, version 0.1.0.

## Purpose

Assemble the draft daily report for one wrapped shoot day from the call sheet, the timecard export, the department reports and the production notes: the day at a glance, the work planned and reported, schedule changes, hours totaled as written by department and for the day, and every missing, incomplete, overlapping or mismatched entry written as a numbered query. The assistant prepares; it never fills in a missing time, corrects an entry, applies a pay rule, resolves a dispute, sends the report or submits anything to payroll.

## When to use it and when not to

Use it once a shoot day has wrapped and the department records are arriving. Run it again when a late card or a corrected entry comes in.

Do not use it:

- for pay. It applies no pay rule, overtime, meal-penalty or guild computation and submits nothing to payroll. Hours are the hours as written. A pay period belongs in Payroll preparation and timesheet review, prepared for the payroll specialist;
- to report a project across weeks. That is Project status report;
- to re-plan the shoot schedule after a change. This capability notes the change as written; it does not re-plan around it;
- for more than one shoot day in one run. Run it once per day.

## Roles

- **Runs it:** the production coordinator.
- **Checks the report and decides what goes out:** the production manager.
- **Answers a query:** the person or department head named beside it.
- **Applies pay rules and approves any payroll or guild submission:** the payroll specialist, outside this capability.
- **Receives the approved report:** the production office, department heads and cost reporting, as the production manager decides.

## Inputs

1. **The call sheet.** The production name, the shoot day, the date, the location, the general call, the planned wrap and the planned work, then the crew list with these default headers: `name,department,position,call_time`. If there is no call sheet, stop and ask.
2. **The timecard export** for the day, one row per entry, with these default headers: `name,department,position,call_in,wrap_out,meal_minutes,hours_logged,note`. Times are 24-hour `hh:mm`. `hours_logged` is hours and minutes (`11:30`) or decimal hours (`11.5`). If the headers do not match, stop and ask which column is which; never guess. If there is no export, stop and ask.
3. **The department reports,** as written by each department head. A department with a timecard and no report is shown as "no report supplied".
4. **The production notes** for the day, including any schedule change called during it. If missing, write "no production notes supplied" and note no schedule change beyond the times.
5. **The settings:** the report template, if the production has one; the tolerance for hours against times (default 0:15); who receives the report. If there is no report template, use the output format below.

The assistant works from files and notes the person supplies. It needs no connection to payroll or accounting and never asks for a password or a login code. If the export carries pay rates, ID numbers or bank details, it does not repeat them; it tells the person to remove them from the source.

## The procedure

1. **Check the inputs.** Confirm one production, one date and one shoot day. The export is taken to be for the call sheet's date unless it carries a date column. If it has a date column, every row must be for that date; if it holds more than one date or a date that differs from the call sheet, stop and ask. Count the call-sheet people, the timecard rows and the people those rows belong to.
2. **Read the hours as written.** Take `hours_logged` exactly as written, as minutes. Convert decimal hours to minutes (`11.5` is 11:30). If a decimal value does not give a whole number of minutes, do not round it: leave the entry out of every total and add a query that prints the value exactly as written. Blank means unknown: it is never zero, and a blank entry is left out of every total and listed in step 6.
3. **Total as written.** Add the minutes by department and for the day. Print every total as hours and minutes. Count entries, not just people: a person with two entries counts once as a person and twice as entries. Print how many entries the day total includes out of all entries. Round nothing. Apply no deduction, rate or rule.
4. **Compare with the call sheet.** Match people by name exactly as written. A person on the call sheet with no row is a missing timecard. A person with a row and no place on the call sheet is not on the call sheet. If two names look alike but differ, do not decide they are the same person; list both in one query of kind Other (step 6). For each listed person, compare `call_in` with `call_time` (for a person with two entries, use the earlier call-in); report how many match and name each that does not. Find the earliest logged call-in and the latest logged wrap-out.
5. **Check each entry's own arithmetic.** For an entry with call-in, wrap-out and meal minutes all written: the span from call-in to wrap-out, less the written meal minutes, is compared with the hours written. A difference larger than the tolerance is a query that shows the span, the meal, the result and the written hours. This checks the entry against itself and applies no pay rule. If wrap-out is earlier than call-in, do not compute; add a query. If the meal is blank, skip the comparison and add a query.
6. **Find the entries that need a query.** In this fixed order:
   - **Missing timecard:** on the call sheet, no row.
   - **Incomplete entry:** any of call-in, wrap-out or hours blank, or wrap-out earlier than call-in, or a meal blank. Quote the note column.
   - **Overlapping entries:** two rows for one name whose times overlap, or two identical rows. Show both and the overlap in minutes. Total both as written and say the total may count the overlap twice.
   - **Hours differ from times:** from step 5.
   - **Not on the call sheet:** a row with no match, unless the production notes explain the person.
   - **Disputed hours:** any hours the notes or a report describe as disputed, quoted as written.
   - **Other:** anything else in the records that cannot be reconciled, such as a name that differs slightly.
   For each query, state the facts and name who to ask: the person, the department head or the production office. Do not suggest the answer.
7. **Note the schedule.** Compare the planned work and the planned wrap with the department reports and the production notes. List, as written: work planned and not done, work moved to another day and why, a called wrap that differs from the planned wrap and by how much, and any access or booking date, or closing time, the notes give for the next day, listed as a schedule change. List each logged wrap-out later than the called wrap with its time. Describe them only; draw no conclusion about pay. For each planned item use one status word: work moved to another day is "moved to [date]"; work reported done with a gap the department states (a retake, a missing take or element) is "partly done", with the gap stated.
8. **Summarise the department reports.** One line per department, in the department's own facts. Include what it asks for. Add nothing that was not reported. A problem a report states, such as an unreadable card or a missed take, stays in that department's line and is not a query unless it concerns an entry, a person's hours or a dispute. Count only the reports supplied, not departments marked "no report supplied".
9. **Assemble the report** in the production's house format if one was supplied, otherwise in the output format. Every slot in the output format must appear somewhere in a house format; add any the house format lacks at the end. Where a section has nothing, print the line shown for it.
10. **Return the draft** to the production coordinator for the production manager's check. The production manager decides what goes out. Nothing is sent from here.

## Exceptions and stop conditions

- **No call sheet or no timecard export:** stop and ask.
- **Export headers do not match the defaults:** stop and ask which column is which.
- **A date column holding more than one date, or a date that differs from the call sheet:** stop and ask.
- **A name appears on a row with a different department or position from the call sheet:** keep what each source says, show both in one query, and choose neither.
- **Asked to fill in a missing time or hours, drop an overlapping entry, correct a total, or round:** decline; the entry stays as written and the query names who confirms it.
- **Asked for overtime, a meal penalty, a rate, a pay total or any guild computation, or to submit the report or hours to payroll:** decline and name the payroll specialist.
- **Asked to say whether hours are right or whether someone should be paid more or less:** decline; list the facts and the person to ask.
- **A department report names someone in a dispute or a safety incident:** quote what is written in that department's line and add a query naming who follows it up; give no account of your own.
- **The export carries pay rates, ID numbers or bank details:** do not repeat them; tell the person to remove them from the source.

## Output format

```
DAILY PRODUCTION REPORT: [production], shoot day [n] of [total], [weekday date]

For: [production manager]. Prepared from the call sheet ([n] people), the timecard export ([n] entries from [n] people), [n] department reports, the production notes and the settings.
Counts: [n] of the [n] people on the call sheet have a timecard. [n] people with a timecard are not on the call sheet. Queries: [n].

Day at a glance
Location: [location]. General call: [time]. Earliest logged call-in: [time] ([names]).
Planned wrap: [time]. Called wrap: [time / not stated]. Latest logged wrap-out: [time] ([names]).
Call times: the logged call-in matches the call sheet for [n] of the [n] listed people who have a timecard. [Differences: name, call sheet time, logged time. / No differences.]

Work planned and reported
[Item]: [done / partly done / not started / moved to date], with what the departments report. [One line per planned item.]

Department reports
[Department]: [what it reports, including what it asks for / no report supplied].

Schedule changes
[n]. [Change, as written, and its source.] [If none: No schedule change noted.]

Hours as written
[Department]: [n] people, [n] entries, [h:mm / no hours written (see query n)].
Day total: [h:mm], from [n] of the [n] entries. [Entries left out are listed under Queries.]

Queries: [n]
[n]. [Kind.] [The facts, in the entry's own words.] Ask: [person or department].
[If none: No queries.]

Hours disputed in the notes: [quoted / none noted]. Entries whose hours match their times: [n] of [n] ([n] differ, [n] cannot be checked).

Draft for [production manager]'s check. The hours are totaled as written. No pay rule, overtime, meal-penalty or guild computation has been applied, and nothing has been sent or submitted.
```

## Reviewer checklist

1. Every total is recomputed from the export: each department, the day, and the count of entries it includes. (Production manager)
2. Every person on the call sheet is either in the report with hours or in a query. (Production coordinator)
3. Every query has the facts and a name to ask, and none suggests the answer. (Production manager)
4. No blank was filled and no entry was dropped, rounded or corrected. (Production manager)
5. Schedule changes and the called wrap match the production notes. (Production coordinator)
6. Department lines say only what the department wrote. (Department heads)
7. The report applies no pay rule and says so. (Production manager)
8. The report is approved before anything goes to the production office or payroll. (Production manager)

## Acceptance tests

Proposed tests. None has been run.

1. **Clean day.** Every listed person has a card, every card matches its times, no schedule change. Expected: totals by department and day, "No queries", "No schedule change noted".
2. **Missing timecard.** One call-sheet person has no row. Expected: a missing-timecard query; the person is not in any total.
3. **Blank wrap and hours.** Expected: an incomplete-entry query quoting the note; the entry left out of totals and the count of included entries stated.
4. **Overlap.** One person with two entries sharing 30 minutes. Expected: both totaled as written, the overlap in minutes, and a warning that the total may count it twice.
5. **Hours against times.** Hours written 30 minutes above the span less the meal, tolerance 0:15. Expected: a query with the span, meal, result and written hours; total unchanged.
6. **Decimal hours.** `11.5` in the export. Expected: totaled as 11:30.
7. **Header mismatch.** `clock_in` where `call_in` is expected. Expected: stops and asks.
8. **Person not on the call sheet.** Expected: a query; totaled as written.
9. **Two similar names.** "Grip A" on the sheet and "Grip A." on a card. Expected: one query listing both; no assumption.
10. **Asked for overtime or to fill a time.** Expected: declines, names the payroll specialist or the person who confirms.

## Instructions for the AI assistant

```
You assemble the draft daily production report for one shoot day for the
production coordinator. You never fill in a missing time or hours,
correct or drop an entry, apply any pay rule, overtime, meal penalty or
guild computation, send the report, or submit anything to payroll. A
person approves anything that is sent, posted or changed.

The user will supply: the call sheet (production, shoot day, date,
location, general call, planned wrap, planned work, then a crew list with
headers name,department,position,call_time); the timecard export with
headers name,department,position,call_in,wrap_out,meal_minutes,
hours_logged,note; the department reports; the production notes; the
settings (report template, tolerance, default 0:15). If the call sheet
or the export is missing, or the export headers do not match, or the
export holds more than one date or a date that differs from the call
sheet, stop and ask. Confirm first that the inputs are for one
production, one date and one shoot day. Never ask for a password
or a login code.

1. Read hours_logged as written, as minutes (decimal 11.5 is 11:30).
   Blank is unknown, never zero; leave blank entries out of all totals.
   A decimal that is not a whole number of minutes is not rounded: leave
   the entry out of the totals and query it, printing the value.
2. Total as written by department and for the day, as hours and minutes,
   with the count of entries included out of all entries. Round nothing.
3. Match people to the call sheet by exact name. List a missing
   timecard, a person not on the call sheet, and names that look alike
   but differ (one query, no assumption). Report how many logged
   call-ins match the call sheet and name any that do not (for a person
   with two entries, use the earlier call-in).
4. For an entry with call-in, wrap-out and meal written, compare the
   span less the meal with the hours written; above the tolerance, make
   a query showing the arithmetic. Total the written hours anyway.
5. Queries, in this order: missing timecard; incomplete entry (call-in,
   wrap-out, hours or meal blank, or wrap-out earlier than call-in; do
   not compute when wrap-out is earlier than call-in; quote the note);
   overlapping or identical entries (show the overlap; total both as
   written and say it may count twice); hours differ from times; not
   on the call sheet; disputed hours (quoted); other, which also holds a
   department or position that differs from the call sheet (show both,
   choose neither) and a dispute or safety incident in a report (quote it
   and name who follows up). Each states the facts and who to ask.
   Suggest no answer.
6. Schedule changes, as written with their source: work planned and not
   done, work moved and why, called wrap against planned wrap, next-day
   access dates or closing times, and each logged wrap-out later than the
   called wrap. Use one status word per planned item: done, partly done
   (with the gap), not started, or moved to [date]. Draw no conclusion
   about pay.
7. One line per department report, in its own facts; "no report
   supplied" where there is none, not counted as a report. A problem a
   report states stays in its line; it is not a query unless it concerns
   an entry, a person's hours or a dispute.
8. Use the production's report template if given, else the output format
   exactly (the user pastes it with these instructions; if it is not
   there, ask for it), with every slot present and the stated line where a section
   is empty. End with the draft line that says the hours are totaled as
   written, no pay rule has been applied and nothing has been sent or
   submitted.

If asked to fill a time, correct a total, compute overtime, a penalty, a
rate or a guild matter, say whether hours are right, or submit anything,
decline and name the payroll specialist or the person who confirms it.
If the export carries pay rates, ID numbers or bank details, do not
repeat them; tell the user to remove them. Recompute every total before
you return the report.
```

## What to customize

- Your report layout. Keep every slot in the output format.
- The timecard export's headers, and whether hours come as hours and minutes or decimals.
- The tolerance for hours against times (default 0:15).
- Who answers a query for each department.
- How a day is cut when a shoot runs past midnight.
- Who receives the approved report and when.
- Which files the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI. Editorially reviewed. Tried once on its invented example in Claude on 10 November 2026; the record is published with the template and lists the edits made afterward, which have not been run again. Not yet tested in a client environment, and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
