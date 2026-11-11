# Newsletter roundup draft: an invented example

*Illustrative example with invented data.* The Marrowfield Courier is an invented local news publication in an invented town. Its stories, people, companies and links are invented too, and the links point nowhere real. Priya, the newsletter editor, sends a Friday digest of the week's coverage. On Thursday 12 November 2026 she gives the assistant everything below, in full, and gets back the roundup check and the draft that follow.

## What Priya supplied

### 1. Roundup settings

```
Newsletter: The Marrowfield Courier, Friday digest
Today: Thursday 12 November 2026
Send date: Friday 13 November 2026
Approver: Priya (newsletter editor)
Sent by: Marcus (audience producer), once Priya approves
Window: default (published 6 November to 13 November 2026, inclusive)
Item limit: 8. Summary limit: 40 words. Minimum story text: 40 words.
```

### 2. Newsletter format and voice

```
Beat order: Council, Schools, Business, Sport, Arts.
Each item: the story's headline, a summary of one or two sentences, then a
source line with story id, byline, date and link. A lead story, if named,
comes first, above the beats.
Voice: plain words, short sentences, no exclamation marks. We write
"council", never "local authority". Numbers as figures (cardinals; "fourth" stays a word).
Sample item: "The library on Harlow Road will open on Sundays from the new
year. The council said staffing comes from existing budgets."
```

### 3. Editor's priority notes

```
Lead with the bus shelter contract (S1). Keep Sport to one item.
```

### 4. Story index

```
story_id,headline,beat,byline,published,link,status,reuse_note
S1,"Council approves $286,000 bus shelter contract",Council,Hana Whitlock,2026-11-09,https://example.org/courier/bus-shelter-contract,approved,
S2,Council votes to replace Quay Road bus shelters,Council,Joel Brandt,2026-11-09,https://example.org/courier/quay-road-shelters-vote,approved,
S3,Harlow Road Library to open on Sundays,Council,Hana Whitlock,2026-11-10,https://example.org/courier/harlow-library-sundays,approved,
S4,School board delays Eastgate roof repair vote,Schools,Joel Brandt,2026-11-11,https://example.org/courier/eastgate-roof-vote,corrected,"Corrected 12 Nov: the first estimate is $410,000, not $140,000."
S5,Marrowfield High wins regional science prize,Schools,Nia Castellan,2026-11-12,https://example.org/courier/science-prize,approved,Photo supplied by a parent; newsletter use not agreed.
S6,Oven Row to close two shops on 31 December,Business,Nia Castellan,2026-11-10,https://example.org/courier/oven-row-closures,approved,
S7,Harbour Market adds Thursday evening hours,Business,Hana Whitlock,2026-11-06,https://example.org/courier/harbour-market-winter,approved,
S8,Rovers beat Eastfield 3-1 at home,Sport,Joel Brandt,2026-11-08,https://example.org/courier/rovers-eastfield,approved,
S9,Winter lantern festival programme announced,Arts,Nia Castellan,2026-11-12,https://example.org/courier/lantern-festival,approved,
S10,Quay Road pool reopens after repairs,Council,Hana Whitlock,2026-10-28,https://example.org/courier/quay-road-pool,approved,
```

### 5. Story text, as published

```
S1
Marrowfield council voted 7 to 2 on Monday to award the bus shelter contract to Contractor A, at a cost of $286,000. Twelve shelters will be replaced along the Quay Road route, starting in February. Two councillors voted against, saying the cheaper bid should have been taken. The work is expected to take four months.

S2
A split council on Monday approved a $286,000 deal to replace bus shelters along Quay Road. Seven councillors backed the contract and two opposed it. Council officers said the new shelters will have lighting and real-time arrival screens. Installation is planned to begin in February.

S3
Harlow Road Library will open on Sundays from 6 December, from 11 am to 3 pm, the council announced on Tuesday. The change follows a 12-week trial in the summer. Staffing for the extra day comes from the existing library budget, a council spokesperson said. Borrowing and computer use will both be available.

S4
The school board on Tuesday put off a vote on repairing the roof of Eastgate Primary until its December meeting. Members asked for a second estimate. The first estimate puts the cost at $140,000. The board chair said the roof leaks in two classrooms.

S5
Marrowfield High School's science team won the regional prize on Saturday with a project that filters microplastics from washing-machine water. Five students entered. The team goes to the state final in March. Teacher Mr Alvarez said the students built the first version in the school workshop over two terms.

S6
Oven Row, a bakery chain with six shops in the county, will shut its Mill Lane and Station Parade branches on 31 December. Four shops will carry on trading. A company statement says staff at the two closing branches have been offered work at other shops. The Mill Lane branch opened in 2011.

S7
Harbour Market will open on Thursday evenings through the winter, with stalls trading from 4 pm to 8 pm from 19 November to 25 February. The market manager said 22 traders have signed up so far. Hot food stalls will be placed under the covered section.

S8
Marrowfield Rovers beat Eastfield 3 to 1 at home on Saturday, with two of the goals coming in the second half. The win lifts Rovers to fourth in the table, two points behind the leaders. Their next match is away at Dunmore on 21 November.

S9
The programme for this year's Marrowfield Winter Lantern Festival has been announced, with events across

S10
The Quay Road swimming pool will reopen on 2 November after eight weeks of repairs to its filtration system. Lane swimming will be available from 6 am on weekdays. The council said family sessions return the following week, and the changing rooms have been refitted.
```

## What the assistant returned

```
ROUNDUP CHECK: The Marrowfield Courier, Friday digest
For: Priya (newsletter editor). Send date: Friday 13 November 2026. Sent by: Marcus (audience producer).
Prepared 12 November 2026 from 10 index rows, 10 story texts, the format and voice notes and the priority notes. Window: 6 November to 13 November 2026.
Stories in the draft: 7 of a limit of 8.

To settle before this goes out: 5
1. S1 and S2 (Council) both report the 9 November council vote on the Quay Road bus shelter contract. Both are in the draft, each marked as a possible duplicate. S1 names the contractor and the work period; S2 gives the lighting and arrival screens. Should the roundup carry one of them, or both?
2. S4 (Schools) has status "corrected". The note reads: "Corrected 12 Nov: the first estimate is $410,000, not $140,000." The text supplied still says $140,000. Can you send the corrected text, and should the roundup show the correction line?
3. S5 (Schools) has a reuse note: "Photo supplied by a parent; newsletter use not agreed." The draft carries no photo. Can the item run as summarized?
4. S9 (Arts) has 15 words of text, ending after "events across". Can you send the full story?
5. S10 (Council) was published 28 October 2026, before the window opens on 6 November. Should it run in this roundup?

Left out of the draft: 3
- S4 (Schools, corrected): status is corrected. Stays out until question 2 is answered.
- S9 (Arts, incomplete): text is shorter than the minimum of 40 words and ends mid-sentence. Stays out until the full text arrives (question 4).
- S10 (Council, outside the window): published before 6 November 2026. Stays out unless you say it should run (question 5).

NOT READY TO SEND: 5 items to settle.

THE MARROWFIELD COURIER: Friday digest, 13 November 2026
DRAFT. NOT READY TO SEND: 5 items to settle (see the roundup check).

In this roundup: 7 stories. Lead 1, Council 2, Schools 1, Business 2, Sport 1, Arts 0.

LEAD STORY
Council approves $286,000 bus shelter contract
On Monday council voted 7 to 2 to give Contractor A a $286,000 contract to replace 12 shelters on the Quay Road route. Work starts in February and is expected to take 4 months.
S1 · Hana Whitlock · 9 November 2026 · https://example.org/courier/bus-shelter-contract
POSSIBLE DUPLICATE OF S2

COUNCIL
Harlow Road Library to open on Sundays
From 6 December Harlow Road Library will be open on Sundays, 11 am to 3 pm, after a 12-week trial this summer. A council spokesperson said staffing for the extra day comes from the existing library budget.
S3 · Hana Whitlock · 10 November 2026 · https://example.org/courier/harlow-library-sundays

Council votes to replace Quay Road bus shelters
A split council backed the $286,000 contract on Monday, with 7 councillors in favour and 2 against. Officers say the new shelters will include lighting and real-time arrival screens, and installation is due to begin in February.
S2 · Joel Brandt · 9 November 2026 · https://example.org/courier/quay-road-shelters-vote
POSSIBLE DUPLICATE OF S1

SCHOOLS
Marrowfield High wins regional science prize
On Saturday the Marrowfield High School science team took the regional prize for a project to filter microplastics out of washing-machine water. The team, which entered 5 students, goes on to the state final in March.
S5 · Nia Castellan · 12 November 2026 · https://example.org/courier/science-prize
CHECK PERMISSION: Photo supplied by a parent; newsletter use not agreed.

BUSINESS
Oven Row to close two shops on 31 December
On 31 December Oven Row will close the Mill Lane and Station Parade branches; its other 4 county shops stay open. The company says staff at both branches have been offered work elsewhere in the chain.
S6 · Nia Castellan · 10 November 2026 · https://example.org/courier/oven-row-closures

Harbour Market adds Thursday evening hours
From 19 November to 25 February Harbour Market will trade on Thursday evenings, between 4 pm and 8 pm. The manager says 22 traders have so far signed up, and hot food stalls will be under cover.
S7 · Hana Whitlock · 6 November 2026 · https://example.org/courier/harbour-market-winter

SPORT
Rovers beat Eastfield 3-1 at home
Marrowfield Rovers won 3 to 1 at home against Eastfield on Saturday, with 2 goals after the break. They are now fourth, 2 points behind the leaders, and play away at Dunmore on 21 November.
S8 · Joel Brandt · 8 November 2026 · https://example.org/courier/rovers-eastfield

ARTS
Nothing selected for this edition.

Draft for Priya (newsletter editor) to approve. Nothing has been sent or scheduled.
```

Every summary traces to the story text supplied under its identifier, and every date, figure and link is copied from the index or the text. The assistant sent nothing, scheduled nothing and changed no story.
