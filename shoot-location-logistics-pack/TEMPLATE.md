# Shoot location logistics pack

Capability template, version 0.1.0.

## Purpose

Prepare the logistics brief for one location that has joined the shooting schedule: how people and vehicles get in against each day's call and wrap, where the unit parks, what power and facilities the place offers against what departments asked for, who the contacts are, what each department requested and whether the notes answer it, and the status of the agreement, permits, insurance and safety review as the production office states it. Every item on the production's own checklist is matched to a confirmation or listed as unconfirmed, with its owner and the date the requesting department gave. The assistant prepares; it never books, pays, sends, contacts anyone or changes a record, and it decides nothing about permits, safety or insurance.

## When to use it and when not to

Use it when a location is added to the shooting schedule, and run it again whenever the schedule, a department request, the location notes or a confirmation changes, with the last version beside it.

Do not use it:

- to read a location agreement for its terms or to say what it permits. The brief shows only the status the production office gives;
- to judge whether a hazard, a permit, a safety plan or an insurance cover is adequate. Those go to the qualified reviewers;
- to plan a whole event, a trip or a safety induction. Those have their own capabilities, event plan, business trip plan and site safety induction pack;
- to book a space, apply for a permit, notify a neighbour or contact a supplier. People do that.

## Roles

- **Runs it:** the location manager, or the production coordinator for them.
- **Verifies the arrangements and settles every question:** the location manager, with the production manager.
- **Owns each checklist item:** the role in the `owner` column of the checklist.
- **Decides on permits, safety and insurance:** the qualified reviewers the production names. The assistant never does.
- **Receives the approved brief:** department heads, transport and the production office.

## Inputs

1. **The shoot brief.** Production name, location name, each shoot day with its call and wrap time, the number of people (crew and cast), today's date, the location manager and the person who verifies with them. If the location, a shoot day or its call and wrap are missing, stop and ask. If the unit size is missing, write "unit size not supplied" and continue.
2. **The approved location notes,** in the location manager's own words: gate and entry sizes, hours, parking, power, facilities, neighbours, restrictions. Use only what the notes say. If missing, stop and ask.
3. **The production's location checklist.** Default headers: `section`, `item`, `owner`. Default sections: access, parking, equipment and facilities, contacts, department requests, permissions. If the headers do not match, stop and ask which column holds which before using the list. Never add, remove or reword an item. If missing, stop and ask.
4. **The department requests.** Default headers: `department`, `request`, `needed by`, `requested by`. Dates as year-month-day. If the headers do not match, stop and ask. If missing, write "no department requests supplied" and continue.
5. **The contacts list.** Default headers: `name`, `role`, `organisation`, `how to reach`. If the headers do not match, stop and ask. If missing, write "no contacts supplied".
6. **The confirmations log.** Default headers: `item`, `confirmed by`, `date`, `how`. An item is confirmed only when a row names who confirmed it and on what date. If the headers do not match, stop and ask. If missing, write "no confirmations log supplied" and treat every item as unconfirmed.
7. **The status of the agreement, permits, insurance and safety review,** one line each, as the production office states it. Print each exactly as given. If a line is missing, write "status not supplied".
8. **The last version of the brief,** when it is run again. Lines marked confirmed in the log stay confirmed; every change since it is listed in section 1, one line each beginning "Changed:". On a first run there is no last version.

The assistant works from what the person supplies. It needs no access to any calendar, booking system, mailbox or record, and never asks for a password or a login code.

## The procedure

1. **Open the brief.** Count calendar days from today to the first shoot day. List the unit size.
2. **Access.** State the entry (gate or door, widths and heights as noted), the key holder, and the opening hours. For each shoot day compare the call and wrap with the hours: covered only if the hours begin at or before the call and end at or after the wrap. When not covered, state the number of minutes short at each end. Compare every vehicle height in the requests with the lowest height noted on the route and state the difference in metres. Anything not noted is "not noted", never assumed.
3. **Parking.** State the spaces noted and who counted them. Count the vehicles named in the requests, listing each. State the shortfall or spare spaces as a number. State what the notes say about street parking and about crew cars and a unit base, or "no information supplied".
4. **Equipment and facilities.** Power: supply noted against the requests, with the gap as a number in the same unit; say if the notes call it untested. Generator or fixed equipment: what the notes say about position and noise, or "not noted". Toilets, roofed space and rooms for changing or eating: the number or size noted against the number of people and the requests. Do not judge whether a number is enough; state both and leave it to the managers.
5. **Contacts.** Give the on-site contact and key holder, the owner or their representative, and a neighbour contact. A contact is "confirmed" only if the log names who confirmed it and when. A role with nobody named reads "none named". Do not search for or invent a contact.
6. **Department requests.** Give each request one status: *answered* (the notes settle it, naming the note), *open* (the notes do not settle it, saying what is missing), or *conflict* (a number or size in the notes cannot meet it, stating both). A request that offers alternatives ("this or that") is a conflict only when the notes show that every alternative falls short; if any alternative is not settled either way by the notes, it is open. Print the counts.
7. **Items for escalation.** List, with the owner from the checklist ("not named on the checklist" if none), each line from input 7 that is not stated as signed or confirmed, each printed as given, and a notice to neighbours that the notes call unsent if input 7 does not already carry it. Then add one line for each specialist word that appears in any request, naming every request it appears in, marked "for a qualified reviewer", with no assessment. A hazard named in several requests is one line. Its owner is the `requested by` role of the first request, in the order supplied, that names it. Default specialist words: generator, working at height, rigging, fire or flame effects, drone, road closure, water, animals, children, stunts. Replace with the production's own list.
8. **Match the checklist.** Take every checklist item in its order. Confirmed: a log row exists and no request or note contradicts it. Unconfirmed: any other case, with the reason in a few words. A log row matches a checklist item by meaning where the words differ, but it confirms only the thing it names (a measured route does not confirm a vehicle height). An item with a log row that a request or note contradicts is unconfirmed with the conflict stated. Not applicable: only if the production office has said so in the inputs. After the list, name what the requests, notes or status lines raise that is not on the checklist, each once (a notice to neighbours that is unsent counts as one such item, even though it also appears in section 7); suggest it for the checklist and leave the checklist unchanged.
9. **List the unconfirmed items.** One numbered line for every unconfirmed checklist item and every item raised outside the checklist: what is needed, the owner from the checklist (or "not named on the checklist"), and the needed-by date with the days from today. The date comes only from a request that asks for the thing the item is about (a vehicle count for the vehicle-space item, a height for load-in, power for the power item, room for a generator for the generator item, covered space for catering, owner approval for the art item, a quiet period for the quiet-period item, a changing room for the changing-room item). A request that names the thing only in passing (a generator trailer in a list of vehicles) or asks for something else (a quiet period is not a neighbour contact) gives it no date. If two requests ask for the same thing, take the earlier date. With no such request: "none given". Sort by needed-by date, soonest first. Items with the same date keep checklist order and items outside the checklist follow the checklist items. Items with no date come last in checklist order.
10. **Questions for the managers.** Turn the conflicts, the open requests and the escalations into at most six questions, each with its facts, addressed to a role. Write each as a plain question that offers no option: propose no answer and no time, route, vehicle or arrangement not already in the inputs.
11. **Count and close.** Fill the readiness line: checklist items, confirmed, unconfirmed, not applicable, items outside the checklist, total on the unconfirmed list, items for escalation. Use the closing line exactly.

## Exceptions and stop conditions

- **Location, shoot days, call and wrap, notes or checklist missing:** stop and ask.
- **A header does not match the default:** stop and ask which column is which.
- **A call or wrap time that cannot be read, or a wrap before the call:** stop and ask.
- **Two sources disagree** (for instance a space count in the notes and in a request): show both, mark the item unconfirmed and ask which holds.
- **A date is in the past:** list the item as overdue by that many days; do not drop it.
- **An item has no owner on the checklist:** print "Owner: not named on the checklist".
- **Asked to book, apply, notify, contact someone, say a permit, insurance or safety matter is fine, interpret an agreement, or mark an item confirmed without a log row:** decline. People do these.

## Output format

```
LOCATION LOGISTICS BRIEF: [location]. [Production], [shoot days]

Prepared for: [location manager] and [verifier]. Brief date: [date]. First shoot day in [n] days. Unit: [n] people ([crew], [cast]).

1. Readiness
Checklist items: [n]. Confirmed: [n]. Unconfirmed: [n]. Not applicable: [n].
Raised by requests or notes but not on the checklist: [n].
Items on the unconfirmed list: [n]. Items for escalation: [n].
[On a rerun only: Changed: [each change since the last brief], one line each.]

2. Access
Entry: [gate or door, sizes]. Key holder: [name, role, confirmed date or "not confirmed"]. Open: [hours].
[Each shoot day]: call [time] and wrap [time] against [hours]. [Covered, or the minutes short at each end.]
Vehicle height: [request height against lowest height noted, difference in metres, or "not noted"].

3. Parking
Spaces noted: [n] ([who counted, date]). Vehicles requested: [n] ([each]). [Shortfall or spare spaces: n.]
Street parking: [what the notes say]. Crew cars and unit base: [what the notes say or "no information supplied"].

4. Equipment and facilities
Power: [supply noted] against [request]. Gap: [number and unit]. [Untested, if the notes say so.] Generator position and noise: [what the notes say or "not noted"].
Toilets: [number noted] for [n] people. Roofed space: [noted] against the catering request. Changing room: [noted] against the costume request.

5. Contacts
On-site contact and key holder: [name, role, organisation, how to reach, confirmed date or "not confirmed"].
Owner or representative: [same].
Neighbour contact: [same, or "none named"].

6. Department requests
[n] requests. Answered by the notes: [n]. Open: [n]. Conflict: [n].
- [Department]: [answered, open or conflict]. [The note, what is missing, or both figures.]

7. Items for escalation (not treated as ready)
- [Item]: [status as supplied]. Owner: [role]. [For a qualified reviewer, where the specialist list applies.]

8. Checklist matched
[n]. [section]: [item]. [Confirmed: who, date. Unconfirmed: reason. Not applicable: who said so.]
Not on the checklist: [items raised by requests or notes, suggested for the checklist, or "None."]

9. Unconfirmed items ([n]), soonest needed-by first
[n]. [Item] ([checklist number or "not on the checklist"]): [what is needed]. Owner: [role]. Needed by [date] ([n] days), or "Needed by: none given".

10. Questions for the managers
[n]. [Role]: [question with its facts.]

This brief changes no record, books nothing and sends nothing. [Location manager] and [verifier] verify the arrangements. Permits, safety and insurance stay with the people responsible for them.
```

Print "None." under any section with nothing to show. Keep the numbering and the section order.

## Reviewer checklist

1. Every gate hour, call, wrap and minute shortfall matches the notes and the shoot brief. (Location manager)
2. Every count (spaces, vehicles, power, toilets) matches its source and the gap is arithmetically right. (Location manager)
3. Every item marked confirmed has a log row with a name and a date. (Production coordinator)
4. Every checklist item appears once, unchanged, in the checklist matched. (Production coordinator)
5. The unconfirmed list holds every unconfirmed item and is sorted as the rules say. (Production manager)
6. Nothing about permits, safety or insurance is stated as settled, and no agreement term is quoted. (Production manager)
7. Each department request has a status and the counts add up. (Location manager)

## Acceptance tests

Proposed tests. None has been run.

1. **Gate hours.** Hours 07:30 to 18:00; call 07:00, wrap 18:30. Expected: not covered, 30 minutes short at each end.
2. **Vehicles against spaces.** Seven vehicles listed, six spaces. Expected: shortfall 1, each vehicle listed.
3. **Height conflict.** Arch 3.4 m, truck 3.6 m. Expected: 0.2 m over; the checklist item unconfirmed with the conflict stated even though the route was measured.
4. **Header mismatch.** The checklist has columns `area`, `task`, `who`. Expected: stops and asks which column is which.
5. **No log row.** A caretaker "should be fine" in the notes. Expected: unconfirmed; the brief never marks it confirmed.
6. **Specialist word.** A request for a generator trailer. Expected: listed for a qualified reviewer, no assessment.
7. **Asked to book.** "Book the parking for us." Expected: declines and names the person who books.
8. **Past date.** A request needed by a date before today. Expected: kept on the list, marked overdue by the number of days.
9. **Empty section.** No contacts supplied. Expected: "no contacts supplied" in the contacts section and "none named" for each role.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above.

```
You prepare the location logistics brief for the location manager. You
never book, apply, pay, notify, send or contact anyone, you never change a
record, and you decide nothing about permits, safety or insurance. A person
approves everything that leaves the production. You never ask for a
password or a login code.

The user will supply: the shoot brief; the approved location notes; the
production's location checklist; the department requests; the contacts
list; the confirmations log; the status of the agreement, permits,
insurance and safety review; the last brief, if any. If the location,
shoot days with call and wrap, notes or checklist are missing, stop and
ask. If a table's headers differ from the defaults (checklist: section,
item, owner; requests: department, request, needed by, requested by;
contacts: name, role, organisation, how to reach; log: item, confirmed by,
date, how), stop and ask which column is which. If the requests,
contacts or log are missing, write "no department requests supplied",
"no contacts supplied" or "no confirmations log supplied". With no log,
treat every item as unconfirmed. A missing status line reads "status not
supplied".

1. Count days from today to the first shoot day.
2. Access: compare each day's call and wrap with the opening hours; state
   minutes short at each end. A call or wrap you cannot read, or a wrap
   before the call, is a stop: ask. Compare vehicle heights with the lowest
   height noted. Anything the notes do not say is "not noted"; never assume.
   A missing unit size reads "unit size not supplied"; continue.
3. Parking: spaces against vehicles, as a number. If two sources give
   different counts, show both, mark the item unconfirmed and ask which holds.
4. Equipment and facilities: supply against request with the gap; state
   numbers and do not judge whether they are enough. Generator position and
   noise read "not noted" when the notes are silent.
5. Contacts: confirmed only if the log names who and when; else "none
   named" or "not confirmed".
6. Department requests: give each one status. Answered: the notes settle
   it, naming the note. Open: the notes do not settle it, saying what is
   missing. Conflict: a number or size in the notes cannot meet it, stating
   both. A request that offers alternatives is a conflict only if the notes
   show every alternative falls short; otherwise it is open. Print counts.
7. Escalation: every status line (agreement, permits, insurance, safety,
   notice to neighbours) not stated as signed or confirmed, printed exactly
   as given, with its owner from the checklist ("Owner: not named on the
   checklist" if none). Then one line per specialist word found in any
   request (generator, working at height, rigging, fire or flame effects,
   drone, road closure, water, animals, children, stunts), naming every
   request it appears in, marked for a qualified reviewer, with no
   assessment; its owner is the requested-by role of the first request that
   names it. A hazard named in several requests is one line.
8. Match every checklist item in order: confirmed only with a log row (matched
   by meaning; a row confirms only what it names) and no contradiction;
   otherwise unconfirmed with the reason. Not applicable only if the
   production office has said so in the inputs. Name items raised outside the
   checklist, each once (an unsent notice to neighbours is one); do not
   alter the checklist.
9. Number the unconfirmed list: every unconfirmed checklist item and every
   item outside it. The needed-by date comes only from a request that asks
   for that very thing, with the days from today in brackets, for example
   "Needed by 12 November (2 days)" (a generator trailer named in a list
   of vehicles dates only the vehicle spaces; a quiet period dates no
   contact); two such requests, take the earlier; none, "Needed by: none given". Sort by
   needed-by date, ties in checklist order, outside items after the
   checklist items, undated last in checklist order then outside items. A
   date before today is listed as overdue by that many days.
10. At most six questions to named roles, each with its facts, as plain
    questions that offer no option, answer, time or arrangement not already
    in the inputs.
11. Fill the readiness line and use the closing line exactly.

On a rerun with the last brief: lines the log still confirms stay
confirmed; list every change since it under the readiness line, one line
each beginning "Changed:".

Use the output format exactly. Print "None." for an empty section. Do not
read an agreement for its terms or treat any permission as given. If asked
to book, notify, contact someone, call a matter settled or mark an item
confirmed without a log row, decline and name the person who does it.
Never adjust a figure to look better.
```

## What to customize

- Your checklist sections and items, or a one-time mapping of your column headers.
- The specialist words that send a request to a qualified reviewer.
- Who verifies each section, and how many days before the first shoot day the brief is due.
- The statuses your office uses for the agreement, permits, insurance and safety review.
- Who receives the approved brief, and in what form.
- Which notes and lists the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI from its own published map of the work. Tried on its invented example on 10 November 2026 in Claude; the record is published with it. The instructions were revised after review and run again on the same example by the session that revised them. Not yet tested in a client environment.
