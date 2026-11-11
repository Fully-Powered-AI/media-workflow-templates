# Trial of "Reader correction request brief" on its invented example

- **Product:** Claude, run in Claude Code

Model: Sonnet 5.5 (model ID claude-sonnet-5-5), made by Anthropic. The run was one pass, in one session, by a model that did not write the template.

Date: 2026-11-10

This record covers two runs on the same day. The first, below, was made on the template as first written; its output and observations are kept as recorded. The template was then changed to settle the ambiguities that run found, and a second run, at the end of this record, was made on the changed template. The second run was made by the model that made the changes, which had read the example's published output, so it is not an independent run.

# First run

The inputs are the invented example in `public/example.md` (the reader message, published version, reporting notes, correction policy CP-3 and settings). No client data was used. The instruction block and output format in `member/template.md` were followed on those inputs before the example's published output was read.

## What came out

```
READER CORRECTION REQUEST BRIEF: Publication P, "Old Pier Café to reopen after council backs new lease", CR-2026-041
Status: Internal note for Editor E; draft acknowledgement for Audience lead L to approve. Nothing sent, corrected or recorded.
Received: Thursday 5 November 2026, 09:30, by email to the corrections inbox, from Reader R. Piece: published Wednesday 28 October 2026, byline Reporter M, editor Editor E. Changes since publication: None recorded.
Acknowledgement due: Monday 9 November 2026 (C1: two business days).
Sources: policy CP-3, 1 September 2026; published version as supplied, 28 October 2026 07:00; 4 notes supplied.

WHAT THE READER SENT
1. Fact dispute: "says the council voted 7 to 2. It voted 6 to 3."
   Published: Paragraph 3: "Councillors voted 7 to 2 to grant a ten-year lease, ending a dispute that closed the café in March."
   Reader's evidence: E1, E2. Notes: N1; withheld: N3
2. Fact dispute: "It also says the lease is for ten years. The minutes say five."
   Published: Paragraph 3: "to grant a ten-year lease".
   Reader's evidence: E1, E2. Notes: N2; withheld: N3
3. Credit report: "The photograph at the top of the story is mine. I took it on Wednesday 14 October and sent it to your submissions inbox. You credit it to 'staff'."
   Published: Photo caption: "Photo: Publication P staff" (Found in different words: the reader says "staff").
   Reader's evidence: E3. Notes: N4
4. Remark: "I expect better from a local publication."
   Published: No passage.
   Reader's evidence: None supplied. Notes: none on this point
5. Request about handling: "Please correct the story today."
   Published: No passage.
   Reader's evidence: None supplied. Notes: none on this point

EVIDENCE THE READER SUPPLIED
E1. Pasted extract from the council minutes of Tuesday 27 October 2026, item 6. Says: "Motion carried: 6 for, 3 against. Term: five years, with an option to renew for five years." Concerns: points 1, 2. Status: Read (pasted text; the minutes themselves not seen).
E2. Link to the council minutes (https://example.org/council/minutes-2026-10-27). Says: nothing available to me. Concerns: points 1, 2. Status: Not examined.
E3. Attached file pier_cafe_2026-10-14.jpg, named in the message; the image itself was not supplied. Concerns: point 3. Status: Not examined.

WHAT THE NOTES RECORD
N1, Tuesday 27 October 2026, Reporter M, Council vote: records the council clerk saying by phone at 21:40 that the vote was 7 to 2. Bears on point 1. It differs from E1, which gives 6 for, 3 against.
N2, Tuesday 27 October 2026, Reporter M, Lease term: records the café owner saying the lease is for ten years, and that the lease document was not seen. Bears on point 2. It differs from E1, which gives five years with an option to renew for five.
N3, Tuesday 27 October 2026, Reporter M, Council vote and lease: content withheld. Bears on points 1, 2 by topic only.
N4, Wednesday 28 October 2026, Picture desk, Reader photo: records that a file named pier_cafe_2026-10-14.jpg arrived through the submissions inbox on Friday 23 October, that the sender name was not recorded, and that it was published with the credit "staff". Bears on point 3. The file name matches E3. The published caption reads "Photo: Publication P staff".

FLAGS
None.

QUESTIONS FOR EDITOR E
Q1. Which source does the publication treat as the record of the vote and the lease term: the clerk and the owner (N1, N2) or the minutes (E1, E2)? Points 1, 2.
Q2. Does a cleared note cover the claims? N3 is on the topic of points 1 and 2 and its content is withheld; does it bear on them? Points 1, 2; N3.
Q3. Does the picture desk or production record show who supplied the photograph, and what credit it gives? Point 3; N4, E3.
Q4. For each of points 1, 2 and 3, which do you choose: correct, investigate or leave as published, and who records the choice under C2 and C3? Points 1 to 3.
Q5. The reader asks for a correction today (C4 leaves that decision to you). May the reader be given a date for the outcome? Point 5.

DRAFT ACKNOWLEDGEMENT
Subject: Your message about "Old Pier Café to reopen after council backs new lease" (CR-2026-041)

Dear Reader R,

Thank you for writing to us about "Old Pier Café to reopen after council backs new lease". We received your message on Thursday 5 November.

You raised the council vote count, the length of the lease, and the credit on the photograph, and you asked for the story to be corrected today.

Your message has gone to the responsible editor, who will review it and decide what happens next. We will tell you the outcome.

Audience team, Publication P
Length: 82 words against a limit of 120.

BEFORE SENDING
Approval: Audience lead L approves the wording before it is sent; Assistant A sends it.
Promises in this draft: that the reader will be told the outcome, allowed by C7 (no date given).
Left out, and why: whether the vote, the term or the credit is right (the editor decides, C2, C3); any correction or its wording (C4); a date for the outcome (C7); any mention of notes N1 to N4 (internal, C5); a promise to correct today (not allowed by CP-3).
Not covered by the policy: how to answer the remark in point 4; how to treat a reader's claim to have taken a published photograph.

Prepared for Editor E and Audience lead L. Nothing has been sent, published, corrected or recorded by the assistant.
Not completed, and what is needed: E2 and E3 were not examined; supply the minutes text and the image, or the picture desk record, if the editor wants them reviewed. Otherwise nothing outstanding.
```

## What was observed

Every required part of the output format was produced, in order, and no stop condition was met: the message, published version and policy were present, and the notes table had the default headers.

Compared with the published example:

- The note is very close to the example. Same five points in the same order, same three evidence items, same four note entries, no flags, same deadline (Monday 9 November, C1), and the same two items marked Not examined.
- The example asks one question this run missed: whether "ten-year" means the term alone or the term plus the renewal option that the minutes extract mentions. This run's Q1 to Q5 do not ask it. It is a useful question and the template's step 7 does not prompt for it.
- This run asked whether the editor treats the clerk and owner or the minutes as the record, and the example asks the same.
- This run marked the credit "Found in different words" (the reader says "staff", the caption says "Publication P staff"); the example, when this run was made, gave the caption as the position without a result word (the example now carries "Found in different words" for it). This run also noted that the picture desk note says the credit was "staff" while the caption reads "Publication P staff". The example does not mention that small difference.
- The draft acknowledgement differs in wording, not in substance. Both thank the reader, give the day received, list what was raised without agreeing, say the editor will review and decide, and promise only to tell the reader the outcome (C7). The example says the minutes extract was passed on and omits the same-day request; this run restates the same-day request neutrally and does not mention the extract. The example draft is 80 words, this one 82, both under 120.
- Facts not in the inputs: none were found in this run's output. In the example's output, nothing was found either, apart from small inferences such as "the original minutes not seen" and "by phone" (the note says "Called").

Where the template was ambiguous, and what this run guessed (the step numbers below refer to the template as first written, before the later changes described further down):

1. Step 4 says "described attachments are read". The reader's message only names the attached file. This run treated it as Not examined because no image or description was supplied. The example does the same, but the template does not say a bare file name counts as a file not given.
2. The deadline count does not say whether the day of receipt counts. This run started counting the next day (Friday 6 November is business day 1, Monday 9 November is day 2), as the template's own test 10 implies. The step should say so.
3. Step 6 lists legal claims, but a reader saying "the photograph is mine" is an ownership claim that could become a copyright matter. It is not on the flag list. This run did not flag it and listed it as not covered by the policy, and the checklist item on legal views does not settle whether it should be flagged.
4. N3 has `Cleared` set to no and is on the same topic as points 1 and 2. Step 6 flags anything touching a note "marked protected", but "not cleared" and "protected" are different, and the template does not say which N3 is. This run treated it as withheld, not protected, and raised no flag.
5. Step 7 suggests asking "whether the reader may be given a date for the outcome". Policy rule C7 already says no date is given, so the question is answered by the policy. This run asked it anyway, noting C7, as did the example. The template could say to skip it when the policy already settles it.
6. Step 2 says a request for a correction is a request about handling, but a remark ("I expect better...") and the request share one paragraph. The template says points go in the reader's order. This run first put the request before the remark, then reordered to match the reader's words.
7. Step 5 says to list the notes that "bear on the topic", but does not say how to treat dates that do not fit. N4 is dated 28 October but records an arrival on 23 October. This run simply stated both.
8. Reviewer checklist item 9 ("The decision whether to correct or investigate, and the approval and sending of the reply") is not a check the reviewer makes of the output; it reads like a statement of who decides. It reads awkwardly beside items 1 to 8.
9. The deadline line in the output format reads `([policy rule])`; this run added "two business days" to it. The format does not say whether that is allowed.

Nothing in the run required stopping, and nothing was sent, published or changed.

# Second run, after the template was changed

Model: Sonnet 5.5 (model ID claude-sonnet-5-5), made by Anthropic. One pass, in one session, with the invented inputs in `public/example.md` and the changed instruction block and output format. The model had edited the template and had read the example's published output, so this run shows that the changes hold together, not that a stranger would reach the same note.

What changed in the template between the runs: the day of receipt is not counted; a file named but not supplied is Not examined; a note not cleared is withheld, not protected, and raises no flag by itself; a reader's claim to own a published photograph is a credit report unless the reader raises copyright, payment or a takedown; the question about giving the reader a date is skipped when the policy settles it; a question is prompted where published words and evidence describe a term differently; a policy that gives permitted content but no wording is handled by drafting from the permitted statements and listing the missing wording; reviewer checklist item 9 was reworded; the closing line of the output format now reads "by the AI assistant".

## What came out

```
READER CORRECTION REQUEST BRIEF: Publication P, "Old Pier Café to reopen after council backs new lease", CR-2026-041
Status: Internal note for Editor E; draft acknowledgement for Audience lead L to approve. Nothing sent, corrected or recorded.
Received: Thursday 5 November 2026, 09:30, by email to the corrections inbox, from Reader R. Piece: published Wednesday 28 October 2026, byline Reporter M, editor Editor E. Changes since publication: None recorded.
Acknowledgement due: Monday 9 November 2026 (C1).
Sources: policy CP-3, 1 September 2026; published version as supplied, 28 October 2026; 4 notes supplied.

WHAT THE READER SENT
1. Fact dispute: "says the council voted 7 to 2. It voted 6 to 3."
   Published: Paragraph 3: "Councillors voted 7 to 2 to grant a ten-year lease, ending a dispute that closed the café in March."
   Reader's evidence: E1, E2. Notes: N1; withheld: N3
2. Fact dispute: "It also says the lease is for ten years. The minutes say five."
   Published: Paragraph 3: "to grant a ten-year lease"
   Reader's evidence: E1, E2. Notes: N2; withheld: N3
3. Credit report: "The photograph at the top of the story is mine. I took it on Wednesday 14 October and sent it to your submissions inbox. You credit it to 'staff'."
   Published: Found in different words: Photo caption: "Photo: Publication P staff"
   Reader's evidence: E3. Notes: N4
4. Remark: "I expect better from a local publication."
   Published: No passage.
   Reader's evidence: None supplied. Notes: none on this point
5. Request about handling: "Please correct the story today."
   Published: No passage.
   Reader's evidence: None supplied. Notes: none on this point

EVIDENCE THE READER SUPPLIED
E1. Pasted extract from the council minutes of Tuesday 27 October 2026, item 6. Says: "Motion carried: 6 for, 3 against. Term: five years, with an option to renew for five years." Concerns: points 1, 2. Status: Read (text pasted by the reader; the minutes themselves not seen).
E2. Link to the council minutes (https://example.org/council/minutes-2026-10-27). Says: nothing available to me. Concerns: points 1, 2. Status: Not examined.
E3. Attached file pier_cafe_2026-10-14.jpg, named in the message; the image was not supplied. Says: the reader took the photograph on Wednesday 14 October. Concerns: point 3. Status: Not examined.

WHAT THE NOTES RECORD
N1, Tuesday 27 October 2026, Reporter M, Council vote: records the council clerk saying by phone at 21:40 that the vote was 7 to 2. Bears on point 1. It differs from E1, which gives 6 for, 3 against.
N2, Tuesday 27 October 2026, Reporter M, Lease term: records the café owner saying the lease is for ten years, and that the lease document was not seen. Bears on point 2. It differs from E1, which gives five years with an option to renew for five.
N3, Tuesday 27 October 2026, Reporter M, Council vote and lease: content withheld. Bears on points 1, 2 by topic only.
N4, Wednesday 28 October 2026, Picture desk, Reader photo: records that a file named pier_cafe_2026-10-14.jpg arrived through the submissions inbox on Friday 23 October, that the sender name was not recorded, and that it was published with the credit "staff". Bears on point 3. The file name matches E3.

FLAGS
None.

QUESTIONS FOR EDITOR E
Q1. Which source does the publication treat as the record of the vote and the lease term: the clerk and the owner (N1, N2) or the minutes (E1, E2)? Points 1, 2.
Q2. Does "ten-year" in paragraph 3 describe the term alone, or the term with the renewal option that E1 mentions? Point 2; E1, N2.
Q3. N3 is on the topic of points 1 and 2 and its content is withheld. Does it bear on them? Points 1, 2; N3.
Q4. Does the picture desk or production record show who supplied the photograph, and what credit it gives? Point 3; N4, E3.
Q5. For each of points 1, 2 and 3, which do you choose: correct, investigate or leave as published, and who records the choice under C2, C3 and C4? Points 1 to 3.

DRAFT ACKNOWLEDGEMENT
Subject: Your message about "Old Pier Café to reopen after council backs new lease" (CR-2026-041)
Dear Reader R,

Thank you for writing to us about "Old Pier Café to reopen after council backs new lease". We received your message on Thursday 5 November.

You raised the council vote count, the length of the lease and the credit on the photograph, and you asked for the story to be corrected today.

Your message has gone to the responsible editor, who will review it and decide what happens next. We will tell you the outcome.

Audience team, Publication P
Length: 82 words against a limit of 120.

BEFORE SENDING
Approval: Audience lead L approves the wording before it is sent; Assistant A sends it.
Promises in this draft: that the reader will be told the outcome, allowed by C7 (no date given).
Left out, and why: whether the vote, the term or the credit is right (the editor decides, C2, C3); any correction or its wording (C4); a date for the outcome (C7); any mention of notes N1 to N4 (internal, C5); a promise to correct today (not allowed by CP-3); a reply to the remark in point 4 (nothing in CP-3 covers it).
Not covered by the policy: wording for acknowledgements (CP-3 gives what one may say, C7, and the sign-off, C6, not the words); how to answer the remark in point 4.

Prepared for Editor E and Audience lead L. Nothing has been sent, published, corrected or recorded by the AI assistant.
Not completed, and what is needed: E2 and E3 were not examined; supply the minutes text and the image, or the picture desk record, if the editor wants them reviewed. Otherwise nothing outstanding.
```

## What was observed

- Every part of the output format was produced, in order, and no stop condition was met.
- The deadline was counted from the next business day (Friday 6 November is day 1, Monday 9 November is day 2), as the changed step 8 says, and the line reads "(C1)" without extra words.
- The file named but not supplied (E3) was marked Not examined under the changed input 3 and step 4.
- N3 (not cleared) was treated as withheld and raised no flag, as the changed step 6 says.
- The photograph ownership claim was treated as a credit report and not flagged, as the changed step 6 says.
- The question about giving the reader a date was not asked, because C7 settles it. The question about "ten-year" and the renewal option was asked (Q2), prompted by the new wording in step 7.
- CP-3 gives permitted content (C7) and a sign-off (C6) but no wording. The draft was written from the permitted statements and the gap was listed under "Not covered by the policy".
- The draft names the story's headline in full and restates the same-day request neutrally, where the example's published draft says the minutes extract was passed on. Both stay inside C7 and admit nothing.
- No fact outside the inputs appeared in the output, apart from the small inference "by phone" for a note that says "Called".
- Three ambiguities from the first run were left unchanged in the template: the order of a remark and a request in one paragraph (item 6), the date on N4 that does not fit the note's own date (item 7), and whether the deadline line may carry extra words (item 9). This run left the deadline line as "(C1)" and stated both N4 dates.

Nothing was sent, published or changed.

