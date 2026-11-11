# Newsletter roundup draft: trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-10

This is the record of the second of two runs on 10 November 2026. The inputs were the invented Marrowfield Courier example in `public/example.md`: the settings, format and voice notes, priority notes, ten-row story index and ten story texts. No client data was used. The assistant followed the instruction block in `member/template.md` and the output format once, and nothing was sent, scheduled or changed.

The first run followed an earlier version of the instructions. After an independent review the instructions were revised (the figures rule, the fixed wording for an empty beat, the ordering of questions, questions for every kept-out story, and one blank line between the check and the draft) and the example's dates were corrected so that its "today" falls after every date in its own inputs. The first run's record is replaced by this one. In the first run most summaries ran to three sentences, against the rule of one or two; that was a breach of the rule by the run, not an ambiguity in it.

One thing to know about this trial: the example's own output was visible in the same read as its inputs, so it was not hidden while the draft was written. The summaries below were written from the inputs and the rules, and were compared with the example only afterwards. Treat the match on layout and decisions as less independent than a blind run would be.

## What came out

```
ROUNDUP CHECK: The Marrowfield Courier, Friday digest
For: Priya (newsletter editor). Send date: Friday 13 November 2026. Sent by: Marcus (audience producer).
Prepared 12 November 2026 from 10 index rows, 10 story texts, the format and voice notes and the priority notes. Window: 6 November to 13 November 2026.
Stories in the draft: 7 of a limit of 8.

To settle before this goes out: 5
1. S1 and S2 (Council). Both report the council's 9 November vote on the $286,000 Quay Road bus shelter contract, 7 to 2. Both are in the draft and each is marked as a possible duplicate of the other. Should the roundup carry one of them, or both?
2. S4 (Schools). Status is corrected. The reuse note reads: "Corrected 12 Nov: the first estimate is $410,000, not $140,000." The text supplied still says $140,000. Can you send the corrected text, and should the roundup show the correction?
3. S5 (Schools). The reuse note reads: "Photo supplied by a parent; newsletter use not agreed." The draft carries no photo. Can the item run?
4. S9 (Arts). The text is 15 words and ends after "events across". Can you send the full story?
5. S10 (Council). Published 28 October 2026, before the window opens on 6 November. Should it run in this roundup?

Left out of the draft: 3
- S4 (Schools, corrected): status is corrected and the supplied text gives the old estimate. Stays out until question 2 is answered.
- S9 (Arts, incomplete): 15 words, below the minimum of 40, and it ends without a full stop. Stays out until the full story arrives (question 4).
- S10 (Council, outside the window): published 28 October 2026, before 6 November. Stays out unless you say it should run (question 5).

NOT READY TO SEND: 5 items to settle.

THE MARROWFIELD COURIER: Friday digest, 13 November 2026
DRAFT. NOT READY TO SEND: 5 items to settle (see the roundup check).

In this roundup: 7 stories. Lead 1, Council 2, Schools 1, Business 2, Sport 1, Arts 0.

LEAD STORY
Council approves $286,000 bus shelter contract
On Monday council voted 7 to 2 to award Contractor A the $286,000 contract. Replacement of 12 shelters on the Quay Road route starts in February and is expected to take 4 months.
S1 · Hana Whitlock · 9 November 2026 · https://example.org/courier/bus-shelter-contract
POSSIBLE DUPLICATE OF S2

COUNCIL
Harlow Road Library to open on Sundays
Harlow Road Library will open on Sundays from 6 December, 11 am to 3 pm, after a 12-week trial in the summer. A council spokesperson said staffing comes from the existing library budget.
S3 · Hana Whitlock · 10 November 2026 · https://example.org/courier/harlow-library-sundays

Council votes to replace Quay Road bus shelters
A split council approved the $286,000 contract on Monday, with 7 councillors backing it and 2 opposed. Officers said the new shelters will include lighting and real-time arrival screens, with installation due to begin in February.
S2 · Joel Brandt · 9 November 2026 · https://example.org/courier/quay-road-shelters-vote
POSSIBLE DUPLICATE OF S1

SCHOOLS
Marrowfield High wins regional science prize
On Saturday the school's science team won the regional prize for a project to filter microplastics out of washing-machine water. The team, which entered 5 students, goes to the state final in March.
S5 · Nia Castellan · 12 November 2026 · https://example.org/courier/science-prize
CHECK PERMISSION: Photo supplied by a parent; newsletter use not agreed.

BUSINESS
Oven Row to close two shops on 31 December
Oven Row will close its Mill Lane and Station Parade branches on 31 December, and its other 4 shops will keep trading. The company says it has offered staff at both branches jobs at its other shops.
S6 · Nia Castellan · 10 November 2026 · https://example.org/courier/oven-row-closures

Harbour Market adds Thursday evening hours
Harbour Market will trade on Thursday evenings, 4 pm to 8 pm, from 19 November to 25 February. The market manager said 22 traders have signed up so far.
S7 · Hana Whitlock · 6 November 2026 · https://example.org/courier/harbour-market-winter

SPORT
Rovers beat Eastfield 3-1 at home
Marrowfield Rovers beat Eastfield 3 to 1 at home on Saturday, with 2 of the goals in the second half. They are now fourth, 2 points behind the leaders, and play away at Dunmore on 21 November.
S8 · Joel Brandt · 8 November 2026 · https://example.org/courier/rovers-eastfield

ARTS
Nothing selected for this edition.

Draft for Priya (newsletter editor) to approve. Nothing has been sent or scheduled.
```

## What was observed

Every required part was produced: the roundup check, the questions, the left-out list, the status line, the contents line, the lead story, all five beats in order (Arts empty) and the closing line. Nothing in the template told the assistant to stop; the inputs were complete and the headers matched.

The decisions matched the published example: S1 as lead, S1 and S2 flagged as possible duplicates and both kept, S4 left out as corrected, S9 left out as incomplete, S10 left out as outside the window, S5 kept with a permission flag, Arts printed empty, 7 of 8 in the draft, five questions, in the order of the lowest story number. Council order (S3 before S2, newest first) also matched. The summaries were counted afterwards: each is two sentences and within 40 words. The dates in the inputs are now consistent with the "today" of 12 November, so nothing in them needed a comment.

The house voice's "numbers as figures" and the rule to keep every value unchanged no longer conflicted: the number words in the stories ("Twelve", "Seven", "Five", "Four", "two") became figures with the same values, in the summaries and in the item text, and the sentence that starts with a figure was avoided by rewording. The headline "Oven Row to close two shops on 31 December" is the story's own and was left as published. "Fourth" stayed a word, as the voice note says.

Smaller points where the instructions still leave a choice, and what this run did:

- **Empty bracketed fields.** The check line "[Text with no index row: ...] [Priority notes naming a story not in the index: ...]" does not say whether to print "None" when there are none. This run left both out.
- **The corrected story's source.** The correction wording lives in S4's `reuse_note`, which is the same column that holds S5's permission note. The stated order of reasons handles this, but the template does not say it plainly.
- **A lead story that is also a possible duplicate.** The format allows the duplicate marker on the lead, and this run put it there, but the procedure does not say so in words.
- **The six-word copying limit.** Keeping under it while keeping attribution still takes care, and "a name, a title, a figure or a date" leaves some runs, such as "2 of the goals in the second half", open to judgment. The run checked its sentences against the stories by eye, not by a count.

No defect stopped the run. The output follows the format and the checklist's seven points can all be applied to it. The trial was run twice on invented material, by the same model, in one product; it says nothing about use with a real publication.

## After the review

An independent review of this record led to small edits in `member/template.md` (rules added to the instruction block that the procedure already stated; a note on empty fields; question order described as index order) and in `public/example.md` (the S1 headline quoted in the index; the S3 summary tightened to "staffing for the extra day"; one comma removed). The run above was not repeated for these edits and its output and observations are unchanged; the output above is the run's own, and differs from the example in the S3 summary wording. A blind rerun, where the assistant does not see the example's output, has not been done and would be stronger evidence.
