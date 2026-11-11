# Daily production report: an invented example

*Illustrative example with invented data.* The production, the crew, the times and the notes below are all invented. The production is an invented ten-day shoot of a short film, run by a small production office; people are named by their position and a letter. First come the inputs the production coordinator supplied, in full, then the report the capability returned.

## The inputs

### 1. The call sheet

```
Production: Short film P
Shoot day: 6 of 10
Date: Tuesday 3 March 2026
Location: Location A (warehouse)
General call: 07:00
Planned wrap: 18:00
Planned work: Scene 14, Scene 15, Scene 17

name,department,position,call_time
Camera Operator A,Camera,Camera operator,07:00
Focus Puller A,Camera,1st AC,07:00
Gaffer A,Grip and electric,Gaffer,06:30
Grip A,Grip and electric,Key grip,07:00
Sound Mixer A,Sound,Sound mixer,07:00
Art Assistant A,Art,Art assistant,07:00
Production Assistant A,Production,Production assistant,06:30
Script Supervisor A,Production,Script supervisor,07:00
```

### 2. The timecard export

```
name,department,position,call_in,wrap_out,meal_minutes,hours_logged,note
Camera Operator A,Camera,Camera operator,07:00,18:30,30,11:00,
Focus Puller A,Camera,1st AC,07:00,18:30,30,11:30,
Gaffer A,Grip and electric,Gaffer,06:30,19:00,60,11:30,
Grip A,Grip and electric,Key grip,07:00,19:00,30,11:30,
Sound Mixer A,Sound,Sound mixer,07:00,,30,,left before wrap; to confirm
Art Assistant A,Art,Art assistant,07:00,13:00,30,5:30,
Art Assistant A,Art,Art assistant,12:30,16:00,0,3:30,second set
Production Assistant A,Production,Production assistant,06:30,19:30,60,12:00,
Driver A,Production,Driver,10:00,17:00,30,6:30,
```

### 3. The department reports

```
Camera: Scenes 14 and 15 shot. Scene 17 not started. 22 setups. One camera card was unreadable and two takes of scene 15 were shot again.
Grip and electric: Lighting for scene 17 is rigged and left in place overnight. Generator refuelled at 15:00.
Sound: Scenes 14 and 15 recorded. The wild track for scene 15 was not taken; a pickup is requested.
Art: Dressing for scene 17 is not finished. The door prop arrives tomorrow morning.
Production: no report supplied.
```

### 4. The production notes

```
Scene 17 moved to Wednesday 4 March because the light went at 17:45. Wrap was called at 18:30. Location A access closes at 20:00 tomorrow.
```

### 5. The settings

```
Report template: none supplied; use the template's own layout.
Tolerance for hours against times: 0:15 (the default).
Report goes to: the production manager.
```

## The output

**DAILY PRODUCTION REPORT: Short film P, shoot day 6 of 10, Tuesday 3 March 2026**

- **For:** Production manager. Prepared from the call sheet (8 people), the timecard export (9 entries from 8 people), four department reports, the production notes and the settings.
- **Counts:** 7 of the 8 people on the call sheet have a timecard. 1 person with a timecard is not on the call sheet. Queries: 5.

**Day at a glance**

- **Location:** Location A (warehouse).
- **General call:** 07:00. Earliest logged call-in: 06:30 (Gaffer A, Production Assistant A).
- **Planned wrap:** 18:00. Called wrap: 18:30. Latest logged wrap-out: 19:30 (Production Assistant A).
- **Call times:** the logged call-in matches the call sheet for 7 of the 7 listed people who have a timecard. No differences.

**Work planned and reported**

- **Scene 14:** done (Camera, Sound).
- **Scene 15:** partly done (Camera, Sound). Camera reports one unreadable camera card and two takes shot again. Sound reports the wild track was not taken and asks for a pickup.
- **Scene 17:** moved to Wednesday 4 March (production notes). Grip and electric report the lighting rigged and left in place overnight; Art reports the dressing not finished and the door prop due tomorrow morning.

**Department reports**

- **Camera:** Scenes 14 and 15 shot; scene 17 not started; 22 setups; one camera card unreadable; two takes of scene 15 shot again.
- **Grip and electric:** Lighting for scene 17 rigged and left in place overnight; generator refuelled at 15:00.
- **Sound:** Scenes 14 and 15 recorded; wild track for scene 15 not taken; pickup requested.
- **Art:** Dressing for scene 17 not finished; door prop arrives tomorrow morning.
- **Production:** no report supplied.

**Schedule changes**

1. Scene 17 moved from today to Wednesday 4 March; the light went at 17:45 (production notes).
2. Wrap called at 18:30 against a planned 18:00, 0:30 later (production notes).
3. Logged wrap-outs after the called wrap of 18:30: Gaffer A 19:00, Grip A 19:00, Production Assistant A 19:30.
4. Location A access closes at 20:00 tomorrow (production notes).

**Hours as written**

- **Camera:** 2 people, 2 entries, 22:30.
- **Grip and electric:** 2 people, 2 entries, 23:00.
- **Sound:** 1 person, 1 entry, no hours written (see query 2).
- **Art:** 1 person, 2 entries, 9:00 (see query 3).
- **Production:** 2 people, 2 entries, 18:30.
- **Day total:** 73:00, from 8 of the 9 entries. Entries left out are listed under Queries (the Sound entry, query 2).

**Queries: 5**

1. **Missing timecard.** Script Supervisor A (Production, script supervisor) is on the call sheet with a 07:00 call and has no timecard. Ask: Script Supervisor A, or the production office.
2. **Incomplete entry.** Sound Mixer A (Sound): call-in 07:00 and meal 30 minutes are written; wrap-out and hours are blank. The note reads "left before wrap; to confirm". Not included in any total. Ask: Sound Mixer A.
3. **Overlapping entries.** Art Assistant A (Art) has two entries on the same day: 07:00 to 13:00 (5:30 written) and 12:30 to 16:00 (3:30 written, note "second set"). They overlap from 12:30 to 13:00, 0:30. Both are totaled as written (9:00), so the total may count that 0:30 twice. Ask: Art department head.
4. **Hours differ from times.** Focus Puller A (Camera): 07:00 to 18:30 is 11:30; less the written meal of 0:30 is 11:00. Hours written: 11:30. Difference: 0:30, above the 0:15 tolerance. Totaled as written (11:30). Ask: Focus Puller A, or the Camera department head.
5. **Not on the call sheet.** Driver A (Production, driver) has a timecard, 10:00 to 17:00, 6:30 written, and is not on the call sheet or mentioned in the production notes. Totaled as written. Ask: the production office.

Hours disputed in the notes: none noted. Entries whose hours match their times: 7 of 9 (one differs, query 4; one cannot be checked, query 2).

Draft for the production manager's check. The hours are totaled as written. No pay rule, overtime, meal-penalty or guild computation has been applied, and nothing has been sent or submitted.
