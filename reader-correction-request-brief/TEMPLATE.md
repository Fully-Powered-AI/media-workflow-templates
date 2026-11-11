# Reader correction request brief

Capability template, version 0.1.0.

## Purpose

Turn one reader's message about one published piece into an internal note for the responsible editor, plus a draft acknowledgement for the audience lead to approve. The note splits the message into numbered points, quotes the published words each point refers to, lists the evidence the reader supplied, sets out what the cleared reporting notes record, flags anything another role must handle, and ends with questions for the editor. The AI assistant prepares; the editor decides whether to correct, investigate or leave the piece as published, and the audience lead approves the reply. It never decides whether the reader is right, admits an error, promises a correction, reveals a confidential source or judges a legal question. It never sends, publishes or changes a record.

## When to use it and when not to

Use it when a reader disputes a fact, a figure, a quotation or a name in a published piece, or reports a missing, wrong or misspelled credit. It suits articles, reports, newsletters, captions and credit lines.

Do not use it:

- to answer a customer's order, billing or product question; use customer reply drafting;
- to apply a refund or compensation policy; use complaint and refund request handling;
- to reply publicly to a review; use public guest review reply;
- when the publication has no written correction policy. The acknowledgement would then invent your rules;
- to write the correction itself, or the editor's reasons for a decision.

## Roles

- **Runs it:** the editor's assistant or the audience team member who received the message, and sends the acknowledgement once approved.
- **Decides what happens to the piece:** the responsible editor, named for the piece.
- **Approves the acknowledgement:** the audience lead.
- **Holds the cleared notes:** the reporter or editor who wrote them, who alone decides which notes the AI assistant may read.
- **Handles flagged matters:** the roles named in the settings, such as [your standards role], [your legal-review role] and [your privacy role].

## Inputs

1. **The reader's message,** complete and unedited, with the channel and the date and time received. If missing, stop.
2. **The published version** of the piece as it stands now: headline, byline, publication date, the full text, captions and credit lines, and any recorded corrections or updates. If missing, stop.
3. **What the reader attached or linked.** Pasted text is read. A description of an attachment or link in the reader's own message is recorded as the reader's statement of what it is, not as its content. A link, or a file that the message names but the AI assistant has not been given, is listed as Not examined and never summarized from its address or file name.
4. **The reporting notes the editor will show,** as a table with these default headers: `Note ID`, `Date`, `Author`, `Topic`, `Content`, `Cleared`. A note with `Cleared` set to no may appear with its content blank or marked withheld; the AI assistant uses only its ID, date, author and topic. If a header does not match, stop and ask which column is which. If no notes are supplied, say "no notes supplied" in that section and continue.
5. **The correction policy** with each rule numbered, including who decides, the acknowledgement time, what an acknowledgement may say, any approved wording for acknowledgements and the sign-off. If missing, stop.
6. **Settings:** the responsible editor, the audience lead, the sender, today's date, the days the office is closed ([your closed days]), the length limit for an acknowledgement (default 120 words) and the roles for flagged matters.

## The procedure

1. **Check the inputs.** Confirm the message, the published version and the policy are present and the notes table has the default headers. Note the policy's identifier and date. If the message is about more than one piece, take the first piece named, and list the others on the "Not completed" line for their own runs.
2. **Number the points.** Split the message into separate points, in the reader's order, each close to the reader's words. One sentence can hold two points; a sentence disputing a figure and a date is two. Give each point one kind: fact dispute (a fact, figure, quotation or name is said to be wrong), credit report (a credit is said to be missing, wrong or misspelled), request about handling (what the reader wants done, or by when), or remark (opinion or feeling that asks for nothing checkable). A request for a correction, an apology or a removal is a request about handling.
3. **Locate each point in the published piece.** For fact disputes and credit reports, quote the exact published words with their position (paragraph number, caption, credit line). Give one result: Found (shown as the position and exact words alone, with no result word), Found in different words (quote what is there), Not found in this version, or Changed since publication (quote the recorded change). A point for which the published piece shows nothing to quote, such as a remark, says "No passage".
4. **List the evidence.** Number what the reader supplied (E1, E2, …). For each, say what it is, what it says in the reader's own text, which points it concerns and its status: Read (text supplied) or Not examined (link, or file named but not supplied). Do not rate how reliable it is.
5. **Review the cleared notes.** For each point, list the notes that bear on its topic. For a cleared note, give its ID and what it records, in a short quotation or close summary. Leave out any name or detail that identifies a person who spoke in confidence, and write "[detail left out]" where it was. For a note not cleared, give its ID, date, author and topic and "content withheld". State what a note records; never say that it proves, supports or disproves the reader. If two sources differ, say they differ and where.
6. **Raise flags.** A flag is anything the editor should not hand back to the AI assistant to work out. Flag a mention of a lawyer, a legal claim, a regulator or a threat to sue; a request to remove a piece or a name, or a claim about personal data; a claim of harm to a named person; a request to reveal who a source was; a claim that the reader is themselves the subject of the piece; and any point that touches a note marked protected. A note with `Cleared` set to no is withheld, not protected, and raises no flag by itself; a note is protected only when the settings, the editor or the note's own topic say so. A reader's claim to have taken, own or have permitted a published photograph is a credit report, not a legal claim, unless the reader also raises copyright, payment or a takedown. Name the role from the settings. Draw no conclusion about the substance of a flagged matter.
7. **Write the questions for the editor.** One question per matter that only the editor can settle, each naming the points and sources it concerns. Use the forms that fit: which source the publication treats as the record; whether a cleared note covers the claim; whether the production or picture record shows who supplied something; whether a term the published words use means what the evidence describes (a lease length that the evidence gives with an option, for example); which option of correct, investigate or leave as published the editor chooses for each fact dispute and credit report (and who records that choice, under the policy); and whether the reader may be given a date for the outcome, but only when the policy does not already settle it. Do not suggest which option is right.
8. **Count the acknowledgement deadline.** From the date received, count the business days the policy sets, skipping weekends and [your closed days]. The day of receipt does not count: the next business day is day 1. Give the day and date and the policy rule it comes from. If the policy sets no time, write "not set by policy" and give no date.
9. **Draft the acknowledgement.** Use the policy's approved wording and sign-off, and keep to the length limit. If the policy sets only what an acknowledgement may say, and gives no wording, write the draft from those permitted statements alone, use the sign-off, and list the missing wording under "Not covered by the policy". It may contain: thanks for writing, the day the message was received, a neutral list of what the reader raised (using "you raised" or "you reported", never "you are right" or "you are mistaken"), that the message has gone to the responsible editor, that the editor will review it and decide what happens next, and only what the policy rule allows beyond that. It must not admit an error or imply one, apologize for the piece, promise a correction, a date or an outcome the policy does not allow, name or describe a source, mention a note, quote a note or give any view on a legal question. If a flag applies and the policy has no wording for it, draft only a plain receipt that says the message arrived and who will reply, or write "No acknowledgement drafted" and say why.
10. **Write the "Before sending" lines.** The approval needed and by whom, the deadline from step 8, each promise in the draft with the policy rule that allows it, what was left out and why, and anything the policy does not cover.
11. **Check against the reviewer checklist and return** the note to the responsible editor and the draft to the audience lead. Finish with the "Not completed" line.
12. **Revise on request.** Shorter, plainer, another channel: redo the draft. Any change that adds a statement goes through step 9 again. A new document from the reader starts again at step 4.

## Exceptions and stop conditions

- **No message, published version or policy:** stop and ask.
- **Notes table headers do not match the defaults:** stop and ask which column is which. Do not guess.
- **The reader's quoted words are not in the published version:** mark the point "Not found in this version"; ask the editor whether an earlier version existed; make no claim about what was published before.
- **A note is marked protected, or names a person who spoke in confidence:** use only what the settings allow, never quote it into the draft, and write "[detail left out]" in the note.
- **A flag under step 6 applies:** complete the note with the flag first. The draft is a plain receipt or none, as step 9 says. Route to the role named in the settings.
- **The reader asks who a source was:** record it as a request about handling, flag it, and decline to name or describe any source.
- **Asked to say whether the reader is right, whether the piece was wrong, or whether it will be corrected:** decline. Those are the editor's. Restate the facts and the questions.
- **Asked to send, post, publish, correct the piece, change a record or contact the reader:** decline; the sender acts after approval.
- **Asked for a legal view on defamation, copyright or privacy:** decline; flag to the legal-review role named in the settings.
- **A reader's message contains a password or login code:** do not repeat it; tell the sender to remove it. The acknowledgement never asks a reader for one.

## Output format

```
READER CORRECTION REQUEST BRIEF: [publication], [piece title], [request reference]
Status: Internal note for [responsible editor]; draft acknowledgement for [audience lead] to approve. Nothing sent, corrected or recorded.
Received: [day, date and time], by [channel], from [reader]. Piece: published [day, date], byline [name], editor [name]. Changes since publication: [list | None recorded].
Acknowledgement due: [day and date] ([policy rule]) | not set by policy.
Sources: policy [identifier, date]; published version as supplied [date]; [n] notes supplied.

WHAT THE READER SENT
[n]. [Kind]: "[the point, close to the reader's words]"
     Published: [position and exact words | Found in different words: [quote] | Not found in this version | Changed since publication: [quote] | No passage]
     Reader's evidence: [E-numbers | None supplied]. Notes: [note IDs | none on this point | withheld: IDs]
(If the reader sent nothing that can be numbered: "No point could be identified.")

EVIDENCE THE READER SUPPLIED
E[n]. [What it is]. Says: [what it says in the reader's text]. Concerns: points [n]. Status: [Read | Not examined].
(If none: "None supplied.")

WHAT THE NOTES RECORD
[Note ID], [date], [author], [topic]: [what it records, short | content withheld]. Bears on points [n].
(If none: "No notes supplied" or "No note bears on these points".)

FLAGS
[Flag]: [what in the message or notes triggers it]. Route to [role].
(If none: "None.")

QUESTIONS FOR [RESPONSIBLE EDITOR]
Q[n]. [Question], points [n], sources [E or note IDs].

DRAFT ACKNOWLEDGEMENT
Subject: [subject]
[Text, in the policy's approved wording, signed as the policy sets out]
Length: [n] words against a limit of [n].

BEFORE SENDING
Approval: [audience lead] approves the wording before it is sent; [sender] sends it.
Promises in this draft: [promise], allowed by [policy rule] | None beyond receipt.
Left out, and why: [statement or detail] ([reason or rule])
Not covered by the policy: [item | None]

Prepared for [responsible editor] and [audience lead]. Nothing has been sent, published, corrected or recorded by the AI assistant.
Not completed, and what is needed: [item and what would settle it | Nothing outstanding]
```

## Reviewer checklist

1. Every point the reader raised is numbered, none is merged with another, and each has one kind. (Audience lead)
2. Every quotation from the published piece matches the version supplied, word for word. (Responsible editor)
3. Every note is described as recording something, never as proving or disproving the reader, and no withheld or protected detail appears. (Responsible editor)
4. The evidence list shows which items were read and which were not examined. (Audience lead)
5. Every flag that applies is raised and routed to the role named in the settings. (Audience lead)
6. The questions can be answered by the editor alone and suggest no answer. (Responsible editor)
7. The deadline is counted correctly against the calendar and tied to a policy rule. (Audience lead)
8. The acknowledgement admits nothing, promises nothing the policy does not allow, names no source and gives no legal view. (Audience lead)
9. The note leaves the decision to correct, investigate or leave as published to the editor, and the draft is marked for the audience lead's approval before it is sent. (Responsible editor; audience lead)

## Acceptance tests

Proposed tests. None has been run.

1. **Complete inputs.** Two disputed facts in one sentence and a credit report. Expected: three separate points, each with its published words, evidence and notes; the acknowledgement lists them without agreeing.
2. **Two sources differ.** A cleared note and the reader's evidence give different figures. Expected: both stated as records, the difference stated, a question to the editor, no ruling.
3. **Withheld note.** One note on the topic has content withheld. Expected: its ID, date, author and topic are listed; no content; the acknowledgement does not mention it.
4. **Protected source in a cleared note.** A cleared note names a person who spoke in confidence. Expected: "[detail left out]" in the note; nothing in the draft.
5. **Quoted words not in the piece.** The reader quotes a sentence the version does not contain. Expected: Not found in this version; a question whether an earlier version existed.
6. **Link not supplied.** The reader links a document. Expected: listed as Not examined; no summary of it.
7. **A lawyer is mentioned.** Expected: a flag routed to the legal-review role; a plain receipt or no acknowledgement; no view on the legal question.
8. **Asked who the source was.** Expected: recorded and flagged; no source named or described.
9. **Asked "is the reader right?" or "will we correct it?".** Expected: declined; facts and questions restated.
10. **Deadline across a weekend.** Received Friday afternoon, two business days. Expected: the following Tuesday, tied to the policy rule.
11. **Header mismatch.** The notes table has `Id` and `Text` columns. Expected: stops and asks which column is which.
12. **Policy sets no acknowledgement time.** Expected: "not set by policy" and no date in the note or the draft.
13. **Asked to send.** Expected: declined; the draft returned for approval.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above.

```
You prepare an internal note for a responsible editor and a draft
acknowledgement for an audience lead, from one reader's message about one
published piece. You prepare; people decide. You never decide whether the
reader is right, admit or imply an error, promise a correction, a date or
an outcome, reveal or describe a confidential source, or give a view on a
legal question. You never send, publish, correct or change a record. If
asked to, decline and return the work for approval.

You will receive: the reader's message with its date; the published
version; what the reader attached or linked; the reporting notes the
editor will show, as a table with the headers Note ID, Date, Author,
Topic, Content, Cleared; the correction policy with numbered rules; and
the settings (responsible editor, audience lead, sender, today's date,
closed days, word limit, roles for flagged matters). If the message, the
published version or the policy is missing, stop and ask. If the notes
table's headers do not match, stop and ask which column is which.

1. Split the message into numbered points in the reader's order, close
   to the reader's words. A sentence with two claims is two points. Give
   each one kind: fact dispute, credit report, request about handling,
   or remark. If the message is about more than one piece, take the
   first piece named and list the others on the "Not completed" line.
2. For fact disputes and credit reports, quote the exact published words
   and their position. Result: Found, Found in different words, Not found
   in this version, or Changed since publication. A point with nothing
   to quote, such as a remark, says "No passage". Never claim what an
   earlier version said unless a recorded change shows it.
3. List the reader's evidence as E1, E2, and so on: what it is, what it
   says in the reader's text, the points it concerns, and Read or Not
   examined. A link, or a file the message names but you have not been
   given, is Not examined; do not summarize it. Do not rate its reliability.
4. For each point, list the notes on its topic and what each records.
   Never write that a note proves, supports or disproves the reader. If
   sources differ, say they differ. For a note not cleared, give only its
   ID, date, author and topic and "content withheld". Where a cleared
   note identifies someone who spoke in confidence, write "[detail left
   out]".
5. Raise a flag, with the role from the settings, for any mention of a
   lawyer, legal claim, regulator or threat to sue; a request to remove a
   piece or name or about personal data; a claim of harm to a named
   person; a request to reveal a source; a claim that the reader is the
   subject of the piece; or anything touching a protected note. A note
   not cleared is withheld, not protected, and raises no flag by itself.
   A reader's claim to have taken or own a published photograph is a
   credit report, not a legal claim, unless the reader raises copyright,
   payment or a takedown. Draw no conclusion about a flagged matter.
6. Write questions for the editor: which source is the record, whether a
   cleared note covers the claim, whether a production or picture record
   shows who supplied something, which of correct, investigate or leave
   as published the editor chooses for each point (suggest none),
   whether a term the published words use means what the evidence
   describes, and whether the reader may be given a date (skip that one
   when the policy already settles it).
7. Count the acknowledgement deadline in business days from the date
   received, skipping weekends and the closed days; the day of receipt
   does not count. Tie it to the policy rule. If the policy sets no
   time, write "not set by policy".
8. Draft the acknowledgement in the policy's approved wording within the
   word limit: thanks, the day received, a neutral list of what the
   reader raised, that it has gone to the responsible editor who will
   review it and decide, and only what a policy rule allows beyond that.
   No admission, no apology for the piece, no promise of a correction, no
   source, no note, no legal view. If the policy gives permitted content
   but no wording, write from the permitted statements alone and list
   the missing wording under "Not covered by the policy". If a flag
   applies and the policy has no wording for it, draft a plain receipt
   or none.
9. Use the output format exactly. Print "None" or the stated empty line
   for any empty section. Fill the "Before sending" lines: the approval
   needed, the deadline, each promise with its policy rule, what was left
   out and why, and what the policy does not cover. End with the lines that say nothing has been
   sent, published, corrected or recorded, and what was not completed.

Never ask the reader for a password or login code. Never change the
reader's evidence to fit a conclusion.
```

## What to customize

- Your correction policy, with numbered rules and the wording of your acknowledgement.
- The responsible editor for each kind of piece, and the audience lead.
- [your closed days], the acknowledgement time and the word limit.
- Which reporting notes may be shown, and how a note is marked withheld or protected.
- Whether a reader's claim to own a published photograph, which this template routes as a credit report, should also be shown to [your legal-review role].
- [your standards role], [your legal-review role] and [your privacy role].
- Where the approved note and acknowledgement are kept, and who records the editor's decision.
- Which files the AI assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI. Tried on its invented example in Claude on 10 November 2026; the record is published with it. The template was changed after that first run, to settle the ambiguities the run found, and was run on the example again; the record covers both runs. Not tested in a client environment.
