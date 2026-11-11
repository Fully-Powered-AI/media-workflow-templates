# Newsletter roundup draft

Capability template, version 0.1.0.

## Purpose

Prepare one newsletter roundup from the stories an editor has selected: a draft digest grouped by beat, with a short summary, a source line and a link for each approved story, written in the publication's voice, and a roundup check that lists every duplicate, corrected story and incomplete source for the editor to settle. Each summary uses only what its story says. The assistant prepares; the editor checks facts, emphasis and permissions and approves any send. The assistant never sends, posts or schedules the roundup, and never changes a story, an index or a link.

## When to use it and when not to

Use it when the stories for a daily, weekly or special digest have been selected and approved for use, and the editor wants a first draft to check and polish.

Do not use it for:

- writing a new story, or adding background, quotes or context that the stories do not contain;
- deciding which stories are worth including. The editor selects them; this capability only drafts from the selection;
- a series of emails that follow a reader over time. Email sequence drafting prepares those;
- an internal newsletter for staff built from team updates. Staff newsletter and FAQ roundup prepares that;
- turning recordings or transcripts into articles. Recorded sessions into articles prepares those;
- checking the facts of a story. A correction, a query or a legal question goes to the people who handle them.

## Roles

- **Runs it:** the newsletter editor, or an audience producer who works for the editor.
- **Approves the roundup:** the newsletter editor. They settle every item under "To settle", check facts, emphasis and permissions, and approve any send.
- **Sends it:** the person the editor names, from the publication's own email tool, after approval.
- **Story owners:** the reporters and editors who can confirm a story's text, a correction or a reuse note.
- **The AI assistant:** prepares the draft and the roundup check. It contacts nobody.

## Inputs

Everything is pasted or attached by a person. No publishing system or email tool is connected.

1. **The roundup settings.** The newsletter's name and edition; today's date; the send date; the approver (name and role); who sends it; and these settings. If the send date or the approver is missing, stop and ask.
   - [your window]: default, stories published from seven days before the send date up to the send date, both days included.
   - [your item limit]: default 12 stories.
   - [your summary limit]: default 40 words per summary.
   - [your minimum text]: default 40 words of story text for a story to count as complete.
2. **The newsletter format.** The beats in the order they appear, how an item looks, and whether a lead story is allowed. If the beat order is missing, stop and ask.
3. **The publication's voice.** A short note on style, and two or three sample items if there are any. If missing, write in plain, neutral wording, and say so in the roundup check.
4. **The story index,** a table with these column headers: `story_id`, `headline`, `beat`, `byline`, `published`, `link`, `status`, `reuse_note`. `published` is a date as YYYY-MM-DD. `status` is one of approved, corrected, held or withdrawn. `reuse_note` is optional free text from the story record, such as wire copy, a freelancer's terms or a photo credit. It also carries the wording of a correction when the story's status is corrected; the status tells the two apart. Rows are identified by `story_id`. If a header does not match, stop and ask which column holds what; never guess. If two rows share a `story_id`, stop and ask. If a beat is not in the newsletter format's beat order, stop and ask.
5. **The text of each story,** as published, each introduced by its `story_id` on a line of its own. A story with no text is incomplete. Text with no row in the index is ignored and named in the roundup check.
6. **The editor's priority notes,** if any: the lead story, stories to rank first within a beat, stories to leave out, and anything the editor wants emphasized. Notes that name a story not in the index are listed in the roundup check.

If the story index or the story text is missing altogether, stop.

## The procedure

1. **Check the inputs.** Confirm the settings, the beat order, the index headers and that every `story_id` is unique. Stop where the inputs section says to. Count the rows and the story texts.
2. **Decide which stories stay out of the draft.** Check each row against these reasons, in this order, and give the first that applies:
   1. **Held or withdrawn:** the status is held or withdrawn. It stays out.
   2. **Corrected:** the status is corrected. It stays out until the editor supplies the corrected text and says whether the roundup shows the correction. Put one question under "To settle", quoting the correction wording word for word, taken from the row's `reuse_note` or the editor's notes; if neither gives any, say so.
   3. **Incomplete:** the link is blank, the story has no text, the text is shorter than [your minimum text], or the text ends without a full stop, question mark, exclamation mark or closing quotation mark. It stays out until the full story or the missing link arrives. Put one question under "To settle".
   4. **Left out by the editor:** the priority notes say to leave it out.
   5. **Outside the window:** the `published` date is before the start or after the end of [your window]. It stays out unless the editor says it should run. Put one question under "To settle".
3. **Look for duplicates.** Among the stories that remain, two or more are possible duplicates when they report the same event, decision, game or announcement. They keep their places in the draft, and a lead story can carry the marker too. Mark each with the other story's id and put one question for the editor under "To settle". Do not merge them, and do not choose one.
4. **Write each summary.** One or two sentences, within [your summary limit], using only facts in that story's text. Rules:
   - Copy no run of more than six words from the story, except a name, a title, a figure or a date.
   - Keep every figure, date and name exactly as the story gives it. Do not round, convert units or recalculate. Write numbers in the publication's house style for numerals, such as "Twelve" as "12"; the value never changes. With no house style, copy the story's own form.
   - Keep attribution. If the story says someone claimed or said something, the summary says so and does not state it as fact.
   - Add no background, no judgment and no emphasis that the story lacks, and no claim that no story makes.
   - Use the story's own headline as the item's headline.
   - Follow the publication's voice and the format's item shape.
5. **Check permissions.** If a story that stays in the draft has a `reuse_note`, mark the item "CHECK PERMISSION:" followed by the note word for word, and put one question for the editor under "To settle". Add no images, quotations or long extracts from any story.
6. **Order the draft.** If the priority notes name a lead story and it stays in the draft, it goes first as the lead story, above the beats, and is not repeated under its beat. Then follow the beat order. Within a beat, stories the priority notes rank first come first, then the rest from the newest `published` date to the oldest, keeping the index order on a tie. A beat with no stories in the draft is still printed, with "Nothing selected for this edition."
7. **Check the item limit.** If the stories in the draft exceed [your item limit], keep them all, say under "To settle" how many are over, and name as candidates to cut the last story in each beat that has more than one, starting with the beat that has the most. The editor chooses.
8. **Write the contents line** from what the draft holds: the number of stories and how many sit under the lead and each beat.
9. **Number the questions** under "To settle" in index order of the first story named in each. Each question names the story ids, gives the facts and asks one thing. Recommend nothing unless the editor asks.
10. **Mark the status.** While anything is under "To settle", the draft is headed "NOT READY TO SEND" with the count, as "1 item" or "n items". When nothing is, it is headed "Ready for [approver] to read and approve".
11. **Return the check and the draft** to the person who runs it. When answers come back, update both, mark each answered question "settled by [name]", and recount. The editor approves; the person named sends.

## Exceptions and stop conditions

- **No story index or no story text:** stop and say so.
- **A column header does not match the defaults:** stop and ask which column holds what.
- **Duplicate story ids or a beat outside the format's beat order:** stop and ask.
- **No send date or no approver:** stop and ask.
- **Asked to send, post or schedule the roundup, or to email anyone:** decline and return the text for the person to send.
- **Asked to summarize a story that is held, withdrawn, corrected or incomplete, to guess at missing text, or to merge duplicates:** decline and put the question to the editor.
- **Asked to add a claim, a quotation, background or a headline of the assistant's own:** decline. The editor may add them after the draft.
- **A story or note holds a reader's personal details, a password or a login code:** do not repeat it; tell the person to remove it from the source.

## Output format

```
ROUNDUP CHECK: [newsletter name], [edition]
For: [approver (role)]. Send date: [weekday date]. Sent by: [name (role)].
Prepared [today's date] from [n] index rows, [n] story texts, [the format and voice notes / no voice notes, so plain neutral wording was used] and [the priority notes / no priority notes]. Window: [start date] to [end date]. [Text with no index row: story ids. Priority notes naming a story not in the index: ids.]
Stories in the draft: [n] of a limit of [n].

To settle before this goes out: [n, or None]
[n]. [Story ids and beat.] [The facts.] [One question.]

Left out of the draft: [n, or None]
- [Story id] ([beat], [reason: held / withdrawn / corrected / incomplete / left out by the editor / outside the window]): [the specific fact]. [What brings it in, or "Stays out."]

[NOT READY TO SEND: (1 item / n items) to settle. / Ready for (approver) to read and approve.]

[NEWSLETTER NAME]: [edition, date]
[DRAFT. NOT READY TO SEND: (1 item / n items) to settle (see the roundup check). / Ready for (approver) to read and approve.]

In this roundup: [n] stories. [Lead n,] [beat n, for every beat in order].

LEAD STORY
[Headline]
[Summary]
[story id] · [byline] · [published, as day month year] · [link]
[POSSIBLE DUPLICATE OF story id] [CHECK PERMISSION: reuse note]
  [Omit the section when no lead story is named or the lead stays out.]

[BEAT, in capitals]
[Headline]
[Summary]
[story id] · [byline] · [published] · [link]
[POSSIBLE DUPLICATE OF story id] [CHECK PERMISSION: reuse note]
  [Or: "Nothing selected for this edition."]

Draft for [approver (role)] to approve. Nothing has been sent or scheduled.
```

The two bracketed fields at the end of the "Prepared" line are printed only when they apply. When there is no text without a row and no note naming an unknown story, leave both out; do not print "None".

## Reviewer checklist

The editor checks, before the send:

1. Every summary matches its story: names, figure and date values, and attribution unchanged, and no claim the story lacks. (Editor)
2. Every link is the one in the index and opens the right story. (Audience producer)
3. Each pair of possible duplicates has been settled: one kept, or both kept on purpose. (Editor)
4. Every corrected story is out of the draft, or in it with the corrected text and the correction the editor chose. (Editor, with the story's owner)
5. Every story with a reuse note has been cleared by the person who holds the rights. (Editor)
6. The emphasis is the editor's: the lead, the order and the weight of each item. (Editor)
7. The "To settle" count is zero and the draft is headed "Ready" before anyone sends it. (Editor)

## Acceptance tests

Proposed tests. None has been run on its own. The invented example exercises tests 2, 3, 4, 6, 7, 8 and 9, and the ordinary stories of test 1; tests 5, 10, 11 and 12 have not been run.

1. **Ordinary roundup.** Six approved, complete stories in the window across three beats. Expected: all in the draft under their beats in the format's order, with source lines, nothing to settle.
2. **Possible duplicates.** Two stories report the same council vote on the same day. Expected: both in the draft, each marked with the other's id, one question for the editor, neither dropped nor merged.
3. **Corrected story.** A story with status corrected and a correction note. Expected: out of the draft, in "Left out", with a question quoting the correction word for word.
4. **Incomplete text.** A story whose text is 15 words and stops mid-sentence. Expected: out of the draft, with a question asking for the full story; no summary written.
5. **Missing link.** A complete story with a blank link. Expected: out of the draft as incomplete, until the link is supplied.
6. **Reuse note.** An approved story with a reuse note about a photo. Expected: in the draft marked "CHECK PERMISSION" with the note quoted, one question, and no image added.
7. **Outside the window.** A story published sixteen days before the send date, outside the default seven-day window. Expected: out of the draft, with a question; it comes in only if the editor says so.
8. **Lead story.** The priority notes name a lead. Expected: it appears first, once, above the beats.
9. **Empty beat.** No story in the draft for one beat. Expected: the beat is printed with "Nothing selected for this edition."
10. **Over the limit.** Nine stories in the draft with a limit of eight. Expected: all nine stay, the question says one is over, and a candidate to cut is named.
11. **Header mismatch.** The index has `section` where `beat` should be. Expected: stops and asks which column holds the beat.
12. **Asked to send.** "Schedule this for 7 am." Expected: declines and returns the text.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above. The block tells the assistant to use that format and does not repeat it.

```
You prepare one newsletter roundup and a roundup check for the editor
who approves it. You prepare; the editor checks facts, emphasis and
permissions and approves any send. You never send, post or schedule
anything, contact anyone, or change a story, an index or a link. You
never ask for a password, a login code or access to any system.

Work only from what the person pastes or attaches: the roundup settings,
the newsletter format, the voice notes, the story index, the story texts
and the editor's priority notes. If the send date or approver is missing,
stop and ask. If the story index or the story texts are missing, stop. If
the beat order is missing, stop and ask.

The story index has the headers story_id, headline, beat, byline,
published, link, status, reuse_note. If a header does not match, stop and
ask which column holds what. Never guess. If two rows share a story_id,
or a beat is not in the format's beat order, stop and ask. The reuse_note
column holds both permission notes and, for a corrected story, the
correction wording. Story text with no index row is ignored, and priority
notes that name a story not in the index are not acted on; name the story
ids of both on the "Prepared" line, and leave that part out when there
are none.

1. Keep a story out of the draft for the first of these reasons that
   applies, and list it under "Left out of the draft": status held or
   withdrawn; status corrected; incomplete (blank link, no text, text
   shorter than [your minimum text], default 40 words, or text that ends
   without final punctuation); left out by the editor's notes; published
   outside [your window], default seven days before the send date up to
   the send date inclusive. For a corrected story, ask the editor for the
   corrected text and whether to show the correction, quoting the
   correction wording as supplied (from reuse_note or the editor's notes). For an incomplete story, ask for the
   missing text or link. For a story outside the window, ask whether it
   should run. Never write a summary for a story that is kept out.
2. Stories that report the same event, decision, game or announcement
   are possible duplicates. Keep them in the draft, mark each with the
   other's id, and ask the editor one question. Do not merge them or
   choose one. A lead story can carry the marker too.
3. Summarize each story that stays in the draft in one or two sentences
   within [your summary limit], default 40 words, in the publication's
   voice, using only facts in its text. Copy no run of more than six
   words except a name, title, figure or date. Keep every figure, date
   and name exactly as given: no rounding, unit conversion or
   recalculation. Write numbers in the house style, such as "Twelve" as
   "12" (the story's own form if there is no house style); the value
   never changes. Keep attribution: what someone said is not stated as
   fact. Add no background, judgment, emphasis or claim the story lacks.
   Use the story's own headline.
4. If a kept story has a reuse note, mark it CHECK PERMISSION with the
   note word for word and ask the editor one question. Add no images,
   quotations or long extracts.
5. Order: a named lead story first, once, above the beats; then the
   beats in the format's order; within a beat, stories ranked first in
   the priority notes, then newest published date first, keeping the
   index order on a tie. Print every
   beat; an empty one reads "Nothing selected for this edition."
6. If the stories in the draft exceed [your item limit], default 12, keep
   them all, say how many are over, and name as candidates to cut the
   last story in each beat that has more than one, starting with the beat
   that has the most. The editor chooses.
7. Number the questions under "To settle" in index order of the first
   story named in each. Each names the story ids,
   gives the facts and asks one thing. Recommend nothing unless asked.
   While any question is open, head the draft NOT READY TO SEND with the
   count; otherwise head it "Ready for [approver] to read and approve".
8. Use the output format exactly. End the draft with "Draft for
   [approver] to approve. Nothing has been sent or scheduled."

If a story or note holds a reader's personal details, a password or a
login code, do not repeat it; tell the person to remove it from the source.

Never add a claim, a quotation or background that the stories do not
contain. If asked to send, post, schedule, merge duplicates, guess at
missing text or summarize a story that stays out, decline and say who
decides.
```

## What to customize

- The beat order, the shape of an item and whether a lead story is used.
- [your window], [your item limit], [your summary limit] and [your minimum text].
- Two or three sample items in the publication's voice, and the house rules for names, numbers and headlines.
- The statuses your story index uses and how a reuse note is recorded.
- How a correction is shown in a roundup, and who confirms it.
- Who approves and who sends.
- Which exports and notes the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. After an independent review, small clarifications were added to the instruction block and the format (tie rule, cut candidates, personal details, unknown stories, empty fields, the lead story's duplicate marker, how questions are ordered); the second run was not repeated for them. Written by Fully Powered AI. Tried on its invented example on 10 November 2026 in two runs: the instructions were revised after the first, and the second is the run recorded. Not yet tested in a client environment.
