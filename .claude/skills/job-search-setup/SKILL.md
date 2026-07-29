---
name: job-search-setup
description: "Sets up a personal AI job search system from scratch: interviews the user about their background, target roles and constraints, builds a Job_Search_HQ folder holding their positioning, fact ledger, writing rules, message library, networking CRM and application tracker, then writes seven working skills that use it. Use when someone says 'set up my job search', 'help me build a job search system', 'I want Claude to help me apply for jobs', 'set up my CV and application workflow', 'I am starting a job hunt', or asks how to get started with job search skills. Run this once, first, before any other job search skill."
---

# Set up a job search system

You are building someone a permanent job search system. It has two halves:

- **A folder of facts about them** that never gets invented and never gets lost between sessions.
- **Seven skills** that read those facts and produce CVs, cover letters, outreach messages, networking records and interview prep.

This skill runs once. Everything after it runs off what you write here.

The whole system depends on one rule: **nothing goes into a CV, a letter or a message that is not traceable to something the person actually told you.** The interview below is how you get those facts. Take it seriously and do not rush it.

Every file you need to write is reproduced in full in this document. Write them **exactly as given**. Do not summarise, abridge or improve them. The only things you change are the placeholders in square brackets, which you fill from the interview, and the `HQ` path.

---

## Step 0: Where does this live?

Ask where they want the folder. Suggest a sensible default for their machine: `Documents\Job_Search_HQ` on Windows, `~/Job_Search_HQ` on Mac or Linux.

Call the chosen absolute path `HQ` from here on. Create it, plus these subfolders:

```
HQ/
  Career_System/     the facts and the rules
  Network/           the contacts CRM
  Tracker/           applications
  Output/            finished CVs, letters, briefs
  Source_Material/   their existing CV, job specs, appraisals, anything raw
```

Then ask them to drop any existing CV, LinkedIn export or old cover letters into `Source_Material/`. If they have one, read it before the interview and use it to pre-fill answers so you are confirming rather than asking cold. Say which parts you took from the CV.

---

## Step 1: The interview

Six blocks. **One block per message.** Do not fire thirty questions at once, and do not disappear and come back with a finished folder. After each block, write what you learned into the relevant file straight away, so a dropped session loses at most one block.

If an answer is vague, push once for the specific version. "I improved a process" is not usable. "I cut invoice approval from nine days to four" is.

### Block A: who they are right now

- Name, city, and whether they are open to relocating or want remote.
- Right to work: which countries can they work in without sponsorship, and do they need sponsorship anywhere they are targeting? This decides which roles are worth applying to at all.
- Total years of professional experience.
- What they are doing right now: employed, on notice, redundant, studying, career break.
- If there is a gap in the last two years, ask what it was and how they want it described. Get this now, in a calm moment, not in the middle of an application.

### Block B: the work history

For each role in the last ten to twelve years, most recent first:

- Employer, exact job title, start and end month and year, location.
- What the job actually was, in one sentence a stranger would understand.
- Three to five things they did that mattered. For each, push for: what was the situation, what did they personally do, what changed as a result. Numbers where real numbers exist. Never invent one, and never let them guess at one either. "Roughly a third faster" is fine. A made-up percentage is not.
- Anything they led, owned, built or fixed that nobody asked them to.

Older roles get two lines each, but **get them anyway**. Early roles close date gaps and prove tenure. A CV with an unexplained eight year hole gets rejected on sight.

### Block C: skills, tools and study

- Tools and software they have genuinely used, each with an honest level: used it, competent, strong, expert. Most people undersell and a few oversell. Ask how recently and how heavily for anything claimed as strong.
- Languages spoken, with level.
- Degrees, professional qualifications, certifications, and anything in progress with an expected date.
- Courses that genuinely taught them something they use. Skip the certificate collection.

### Block D: projects and evidence

Anything outside the job description that shows capability: side projects, volunteering, a tool they built, a committee they ran, published writing, a community they organise, freelance work.

For each: what it is, what they did, is it public, is there a link.

These matter most for people changing direction, because they are the only evidence of the new thing.

### Block E: where they are aiming

- Two or three target role types, in their words. If they name six, make them cut it to three. A search aimed at everything lands nowhere.
- Target sectors or company types, and the size of company they want.
- Seniority they are going for, and whether that is a step up, sideways or a deliberate step down.
- What they will not do. Roles, sectors, shift patterns, commutes, anything that has to be a hard no. This becomes the skip list and it saves hours.
- Their honest salary range. It goes in the file so it is settled before a recruiter asks. It never goes in a document.
- The obvious objection an employer will raise about them, in one sentence. Everyone has one. Getting it on paper is how they stop being ambushed by it.

### Block F: voice and rules

- British or American English.
- Anything they never want written in their name. Offer the common ones and let them pick: em dashes, "passionate about", "results-driven", "proven track record", "leverage", "spearheaded", "synergy", exclamation marks.
- How they actually talk: formal, plain, warm, dry. Ask for a sentence or two of something they have written so you can hear it.
- Anything about their history they do not want raised unless asked.

---

## Step 2: Write the Career_System files

Six files. Fill every placeholder from the interview. **Do not leave bracketed placeholder text sitting in a live file.** If something was not covered, write `NOT YET CAPTURED` on that line so it is visibly missing rather than quietly wrong.

### Write `HQ/Career_System/POSITIONING.md`

````markdown
# Positioning

Last updated: [DATE]

This file decides what to apply for and how to pitch. Everything else reads it first.
Keep it to one page. If it grows past that, it has stopped being a decision and become a wish list.

## In one sentence

[Who they are professionally, at their real level, in the words a hiring manager would use.
Shape: "Twelve years in X, most recently doing Y at Z, now moving toward W."]

## Level

Real level: [mid / senior / lead / manager]
Applying at: [same / one step up / deliberate step down]
Years of relevant experience: [N]

If a job description pitches below this level, it is not a safe application, it is a wasted one.
Never let a document describe them as a student, a beginner or a career changer if the years say otherwise.

## Target lanes

Two or three. Not more.

### Lane 1: [name]
- What the roles are called: [actual job titles used in postings]
- Why they are credible for it: [the honest evidence]
- What is missing: [the real gap and how it gets handled]

### Lane 2: [name]
- What the roles are called:
- Why they are credible for it:
- What is missing:

### Lane 3: [name, optional]

## Skip list

Do not spend time on these. If one comes up, say so before doing any work.

- [Role type or sector that is a hard no]
- [Anything requiring a clearance, licence or certification they do not have and cannot get quickly]
- [Anything requiring sponsorship they cannot get]
- [Shift patterns, travel, commute limits]

## Work rights

- Can work without sponsorship in: [countries]
- Needs sponsorship in: [countries]
- Notes: [visa type, expiry, residency clock, anything affecting eligibility such as clearance rules]

## Salary

Range: [floor to target]
Walk-away number: [floor]

This never appears in a CV, a cover letter or a message. It exists so the answer is already decided when a recruiter asks.

## The standing objection

The thing an employer will privately worry about.

Objection: [one sentence]
Answer: [two sentences, honest, no defensiveness, evidence-led]

Use this in a cover letter only when the posting makes the objection unavoidable. Otherwise hold it for interview.

## Search targets

- Applications per week: [N]
- New outreach contacts per week: [N]
- Conversations booked per month: [N]

Outreach volume beats application volume. Most searches stall because the person sent five messages and called it networking.
````

### Write `HQ/Career_System/CAREER_FACTS.md`

Repeat the role block for every role. Repeat the project block for every project.

````markdown
# Career facts

Last updated: [DATE]

The single source of truth. **Nothing appears in a CV, cover letter, LinkedIn profile or message unless it is traceable to this file or was said by the user in the current session.**

If something is not in here, it did not happen. Add it, then use it.

## Contact block

Name:
Location:
Phone:
Email:
LinkedIn:
Portfolio, GitHub or site:

## Professional experience

Most recent first. Full detail for roughly the last ten to twelve years, two lines each for anything older.

### [Employer] - [Exact job title]
[Month Year] to [Month Year or Present] | [Location]

What the role was: [one sentence a stranger would understand]

Achievements:
- [Situation, what they did, what changed. Keep the numbers real or leave them out.]
- [ ]
- [ ]

Scope: [team size, budget, geography, volume, systems owned]
Tools used here: [ ]
Reason for leaving: [interview prep only, never for a document]

### Earlier roles

- **[Employer], [Title], [Year] to [Year].** [One line on what it was and the one thing worth keeping.]

## Skills

Levels are honest. "Used it" means used it. Only write "expert" if they would survive a technical interview on it.

| Skill or tool | Level | Last used | Where |
| --- | --- | --- | --- |
| | | | |

## Languages

| Language | Level |
| --- | --- |
| | |

## Education and qualifications

- **[Qualification], [Institution], [Year].** [Grade if it helps. Relevant modules or dissertation if recent or relevant.]
- **[Certification], [Body], [Year].** [Expiry if it has one.]
- **In progress:** [ ] expected [date]

## Projects and other evidence

### [Project name]
What it is: [ ]
What they did: [ ]
Public? [link, or no]
What it proves: [ ]

## Metrics that are safe to quote

Anything with a number, stated exactly as it can be defended if challenged.

- [ ]

## Things that are NOT true and must never be claimed

Written down so no one drifts into claiming them when a posting asks.

- [Tool they have never used but that appears near their field]
- [Domain experience they do not have]
- [Level of a language, tool or qualification they cannot back]

## Gaps and how they are described

- [Period]: [agreed one-line description]
````

### Write `HQ/Career_System/CV_RULES.md`

````markdown
# CV, letter and profile rules

Last updated: [DATE]

## Voice

- English: [British / American]
- Tone: [plain / formal / warm / dry]
- Never write a sentence the user would not say out loud.

**Banned:**
- [em dashes / passionate about / results-driven / proven track record / leverage / spearheaded / synergy / exclamation marks]

Vary sentence length. Short sentences carry weight only if the sentences around them are longer.

## CV structure

One page for under five years of experience. Two pages above that. Never three.

Order for an experienced hire:

1. **Name and contact block.** No photo, no date of birth, no marital status.
2. **Professional summary.** Two to four sentences. Their real level in the first six words. The two or three things this specific job cares about. No adjective that could describe anyone.
3. **Professional experience.** Reverse chronological. Employer, title, dates, location.
4. **Education.**
5. **Projects.** Only if they add evidence the jobs do not.
6. **Additional information.** Languages, right to work if it is an advantage, anything genuinely relevant.

Education moves above experience only for a recent graduate or a graduate scheme application.

## The bullet framework

Every bullet does three things in one or two lines:

1. **Action.** Start with a past tense verb. Not "responsible for", not "helped with".
2. **How.** What they actually did, with the tool or method named.
3. **Result.** What changed. A number if a real one exists, otherwise a plain statement of the outcome.

> Redesigned the supplier onboarding checklist across four regional teams, cutting time to first order from nine days to four.

Three to five bullets for a recent role, one or two for an old one. Order bullets by relevance to the job being applied for, not by chronology within the role.

**Strong verbs:** built, led, redesigned, negotiated, launched, cut, resolved, automated, standardised, recovered, scaled, migrated, trained, secured, simplified.

**Weak openings to delete:** responsible for, involved in, helped to, worked on, assisted with, tasked with, participated in.

## Third person, no pronouns, on the CV

The CV never says "I". The cover letter does.

## Formatting for screening software

Applicant tracking systems parse structure before a human sees it.

- Single column. No tables, no text boxes, no graphics carrying information.
- Standard headers: Professional Summary, Professional Experience, Education, Projects, Additional Information.
- Nothing important in a header or footer.
- One common font throughout, consistent sizes.
- Dates in a consistent format, month and year.
- Submit as .docx unless the employer asks for PDF.

## Mirroring the job description without lying

Screeners match language. Use the employer's exact term **when the user genuinely did that thing**. If their CV says "worked with regional finance leads" and the posting says "stakeholder management", that is the same fact in the vocabulary being searched for. Switch it.

Do not do this when the employer's term implies something broader, more senior or more specialised than what actually happened. A reader in that field spots a false equivalence instantly, and it costs more than the keyword gains.

Do not stuff. Repeating a phrase from the posting six times makes the CV duller without helping. A wide vocabulary raises the chance of a match.

## Cover letter structure

One page. Same font as the CV. Formal letter layout: sender details, full date, recipient details.

Address a named person. "Dear Hiring Manager" is the fallback, never the default. On a speculative letter a named person is not optional, and it should not go to HR.

1. **Opening.** Why writing, the exact role, where it was seen. Any real connection goes in the first line.
2. **Why this sector and this company.** Around 150 words. If the company name were deleted, it should still be obvious who the letter is addressed to. Generic paragraph two is why most letters fail.
3. **Why this role.** Around 150 words. Show they understand what the job involves day to day.
4. **The three or four things they asked for.** Around 200 to 250 words, each with a specific example. Elaborate, do not copy CV bullets.
5. **Close.** Short, thanks, availability. On a speculative letter, commit to a follow-up call in a named week.

The letter earns its place by carrying motivation, context and evidence the CV cannot. If it restates the CV, it is doing nothing.

## LinkedIn

A different job from the CV. Narrative, first person, about a third the length, and it says what they are looking for. The CV never does that.

- **Headline** decides whether they appear in recruiter search at all. Front-load it: the first 120 characters are what shows in results. Titles they want, not only titles they had.
- **About**: only the first three lines show before "see more". Put the pitch there. 150 to 180 words total, short paragraphs.
- **Experience** bullets: same framework, two lines maximum, each carrying a searchable term.
- **Skills**: up to 50, all searchable. Pinned ones carry the most weight. Pin what they want to be found for.
- Turn off "share profile updates with your network" before an editing session, or every edit notifies everyone.
- Never let the profile contradict the CV. A recruiter reads both.
````

### Write `HQ/Career_System/MESSAGE_LIBRARY.md`

````markdown
# Message library

Last updated: [DATE]

Templates are a starting shape, not a script. Every message needs one line that could only have been written to that person. Without it, it is a blast, and blasts are why outreach gets silence.

## The three moves

Every message does these in order, in under 150 words.

1. **Context.** Who they are, at their real level, in one sentence. Never open with what they want.
2. **Connection.** The researched line. Something that person did, wrote, shipped, said or is dealing with.
3. **Curiosity.** A small, specific ask. Fifteen minutes and a perspective, not a job. Make the yes easy.

Subject lines: six words, specific, no hype, no "quick question".

## Who to write to

Hiring managers and team leads beat recruiters, every time. They own the problem, they are not filtering against a checklist, and an unusual background reads as interesting rather than as a mismatch.

In-house talent acquisition sits in the middle. Agency recruiters are a volume channel, useful but secondary.

Direct email beats a LinkedIn message by a wide margin. If the company email format can be worked out, use it.

---

## 1. Cold email to a hiring manager, no advertised role

> Subject: [Six words naming their specific problem area]
>
> Hi [Name],
>
> I have spent [N] years in [field], most recently [one concrete thing at the last employer].
>
> I read [specific thing: their post, the product launch, the interview, the change hitting their sector] and it matched something I dealt with at [employer], where [one sentence on the same problem].
>
> Would you have fifteen minutes in the next couple of weeks? I am not asking you to have a role open. I want your read on how [specific thing] is playing out at [company].
>
> [Name]

## 2. Response to an advertised role, sent to the manager not the portal

Send two to three days after the portal application, never the same day.

> Subject: [Role title] application, [their name]
>
> Hi [Name],
>
> I applied for the [role] through your careers page on [date]. I wanted to add one thing the form has no room for.
>
> [The single strongest, most specific match between them and this job, in two sentences.]
>
> Happy to talk if it is useful. Either way, good luck with the search.
>
> [Name]

## 3. LinkedIn connection note

300 characters. No CV, no ask, no pitch.

> [Name], I work in [field] and have been following [specific thing]. Would like to stay connected.

## 4. LinkedIn message after they accept

Wait a day. Never message the same minute they accept.

> Thanks for connecting. I noticed [specific thing about their work]. I have been [relevant one-liner about themselves]. If you ever have fifteen minutes, I would like your view on [specific question]. No rush.

## 5. Recruiter email

The only template where a CV is attached to a first message.

> Subject: [Role type], [N] years, [location or right to work]
>
> Hi [Name],
>
> I am a [role] with [N] years in [field], looking at [role types] in [location]. CV attached.
>
> Most relevant: [two lines, the things a recruiter screens on].
>
> [Right to work status in one line, if it is an advantage.]
>
> Do you have anything current that fits, or should I check back?
>
> [Name]

## 6. Referral ask, to someone they actually know

Never ask a stranger for a referral. Ask for a conversation and let the referral follow.

> [Name], [company] have a [role] open and it looks like a real fit. Would you be comfortable passing my CV to the team, or telling me who owns the role? Completely fine if not, and I would rather ask than assume.

## 7. Warm introduction, using someone's name

Send within a week of getting the name. A referred introduction goes cold fast.

> Subject: [Referrer name] suggested I get in touch
>
> Hi [Name],
>
> [Referrer] mentioned you when we spoke about [topic], and suggested I reach out.
>
> [One sentence on themselves.] I am trying to understand [specific question], and [referrer] thought you would have the sharpest view on it.
>
> Fifteen minutes in the next couple of weeks?
>
> [Name]

## 8. Follow-up after silence

One follow-up. Then leave it. Two is persistence, three is a nuisance. Send seven to ten days after the first message.

> Hi [Name], putting this back on top of your inbox in case it got buried. Still would value fifteen minutes on [specific thing]. If now is not the time, no problem at all.

## 9. Thank you after a conversation

Within 24 hours. Reference the one most useful thing they said and one action taken because of it.

> [Name], thank you for the time yesterday. The point about [specific thing they said] changed how I am thinking about [thing]. I have already [concrete action].
>
> I will [do the thing promised]. If [name they mentioned] is worth an approach, I will mention you suggested it.
>
> Thanks again.

## 10. After a rejection

Worth sending. Rejections turn into referrals more often than people expect.

> Thanks for letting me know, and for the time your team put in. If anything closer to [their strength] comes up, I would be glad to hear about it. Good luck with [the person you hired / the project].

## Rules

- Draft only. **The user sends everything themselves.** Never send, submit or post anything.
- No salary figures in any message.
- No CV attached to a first LinkedIn message, ever.
- If the first line could have been sent to fifty people, rewrite it.
- Effort follows priority. An A-priority contact gets real research. A C-priority contact gets the template with one line changed.

## Diagnosing outreach that is not landing

In this order. Name which one it is.

1. **Wrong target.** Messaging recruiters and gatekeepers instead of the people who own the work.
2. **Wrong opening line.** Generic, or signals junior.
3. **Wrong ask.** Asking for a job, or something vague, instead of fifteen minutes on a specific question.
4. **Wrong volume.** Five messages a week is not a search. Ten a week is.
5. **Wrong channel.** A LinkedIn message where an email would have worked.

Under 15% reply rate on cold outreach means the messages need rewriting, not that the market is closed.
````

### Write `HQ/Career_System/NETWORK_CADENCE.md`

````markdown
# Network cadence

Last updated: [DATE]

How often to contact whom, and what the columns in `Network/Contacts.csv` mean.

## Warmth levels

| Warmth | Means | Interval | Next step |
| --- | --- | --- | --- |
| Cold | Identified, never contacted | 7 days | Send the first message |
| Contacted | First message sent, no reply | 10 days | One follow-up, then Dormant |
| Engaged | They replied | 21 days | Convert to a conversation |
| Warm | Had a real conversation | 42 days | Keep alive with something useful |
| Advocate | Referred them or made an introduction | 30 days | Report back on what came of it |
| Dormant | Two follow-ups, no reply | 90 days | One light touch, then close |
| Closed | Clear no, or left the field | none | Nothing |

## Transitions

- First message sent: Cold becomes Contacted.
- They reply: Contacted becomes Engaged.
- A real conversation happens: Engaged becomes Warm.
- They refer or introduce: becomes Advocate.
- Two follow-ups with no reply, or three failed attempts to book: becomes Dormant.
- Clear no, or they left the industry: Closed, no next touch.

A cold contact who sits untouched for a month should be deleted, not carried. A CRM full of people nobody will ever message is just a guilt list.

## Priority

- **A.** Directly hiring, or owns the work in a target company. Real research before every message.
- **B.** In the target sector, useful perspective, not hiring right now.
- **C.** Weak signal, or a favour to someone else. Template with one line changed.

Effort follows priority. Do not spend an hour researching a C.

## Keeping someone warm

A keep-warm touch has to be worth receiving. Send:

- Something they would find useful and probably have not seen.
- A short update on something they advised on. People like knowing their advice landed.
- A congratulation on something real: a launch, a promotion, a funding round.

Do not send "just checking in", "circling back", or anything that is only a reminder that the sender wants something.

## Owed

The most important column. Anything promised and not yet delivered: an introduction, a document, a follow-up, an answer.

Clear these before anything else. An unclosed loop costs more than a missed follow-up.

## Weekly rhythm

A full week is:

- [N] first messages
- All follow-ups that are due
- Two keep-warm touches
- Every logged interaction written up the same day

If more than that is due, drop the C-priorities and push the rest. Do not send twenty rushed messages.

## The columns

**Contacts.csv** - one row per person, current state:
`ContactID, Name, Company, Title, LinkedIn, Email, Lane, Priority, Warmth, Source, FirstContact, LastTouch, NextTouch, IntervalDays, Owed, Notes`

**Interactions.csv** - one row per contact made, append only, never edited:
`InteractionID, ContactID, Date, Channel, Direction, Summary, Signal, Outcome, NextAction, NextActionDate`

`Signal` is the column that matters. Capture the pain point, the tool complaint, the "we keep meaning to", in their own words. Those sentences are what makes the next message land, and what a cover letter to that company should open with.
````

### Write `HQ/Career_System/INTERVIEW_PLAYBOOK.md`

````markdown
# Interview playbook

Last updated: [DATE]

Built once, reused for every interview. Add to it after each one.

## The story bank

Six to eight stories that cover almost every behavioural question. Each written once, properly, then adapted on the day.

Structure each as: **the situation, what I personally did, what changed.** Two minutes spoken. The middle section carries the weight, so it is the longest part. Say "I", not "we", when describing the actions.

Stories to have ready:

1. **Something hard I delivered.** The clearest example of capability.
2. **A conflict with a colleague or stakeholder.** How it was handled, not how they were wrong.
3. **A failure.** Real, owned, with what changed afterwards. A fake failure is transparent and expensive.
4. **Something I improved without being asked.**
5. **Working under a hard deadline or with too few resources.**
6. **Persuading someone senior.**
7. **A time I was wrong and changed my mind.**
8. **Something learned quickly under pressure.**

### Story: [title]
- Situation:
- What I did:
- Result:
- Answers these questions: [list]

## The standing questions

**"Tell me about yourself."** Ninety seconds. Where they are now, the thread running through their career, why this role. Not a chronology. Rehearse this one out loud until it is boring, because it is asked every time and it sets the tone for everything after.

**"Why this company?"** Needs one researched thing that is not on the homepage. Same standard as the cover letter.

**"Why are you leaving?"** Forward-looking, never bitter. What they are moving toward, not what they are escaping. Even if the truth is that they are escaping.

**"What is your biggest weakness?"** A real one, with what is being done about it. Not a strength in costume.

**"Where do you see yourself in five years?"** A direction, not a title.

**"What are your salary expectations?"** Deflect once: ask what the range is for the role. If pressed, give the range from POSITIONING.md. Never a single number, never below the floor.

## The standing objection

From POSITIONING.md. Whatever an employer will quietly worry about: a gap, a switch, a level, a location, a short tenure.

Prepare the answer in three sentences. Acknowledge it plainly, give the evidence, move on. Do not over-explain. Over-explaining is what turns a small concern into a real one.

Objection:
Answer:

## Questions to ask them

Three good ones. Never zero, and never a list of fifteen.

Good questions are specific, show the work has been thought about, and cannot be answered from the careers page:

- What does the first ninety days look like for whoever takes this?
- What is the thing about this role that people underestimate before they start?
- How does this team decide what not to do?
- What would make you look back in a year and say this hire went well?
- What is currently the most annoying part of this process for the team?

Never ask about holiday, hours or benefits before an offer. That conversation happens with HR, after.

## Per-interview prep

For each interview, produce:

1. **The company in one sentence**, plus what it actually sells and to whom.
2. **What changed in the last six months.** Funding, launches, leadership, layoffs, regulation, a competitor move.
3. **Who is on the panel**, their background, and how long they have been there.
4. **Three likely questions** specific to this role and this posting.
5. **Which stories to use** for each.
6. **The one question this panel will ask that is hardest**, and the answer.
7. **The three questions to ask.**

Flag anything that could not be verified. Never present a guess about a company as fact.

## Formats

- **Screening call, 20 to 30 minutes.** Recruiter checking basics: level, salary, location, right to work, notice period. Be efficient and warm. Have the numbers ready.
- **Panel.** Answer to the person who asked, but include the others with eye contact.
- **Technical or task-based.** Ask about the format in advance. It is a reasonable question and it is always answered.
- **Presentation.** Confirm the time limit and stay inside it. Practise out loud, timed, at least twice.

## After

Same day, write down: every question asked, what went badly, anything promised. Send a short thank you within 24 hours to the person who ran it. Add the questions to this file so the next interview starts from a better place.
````

---

## Step 3: Write the three CSV files

Headers only, no example rows. Fake data in a live CRM is worse than an empty one.

`HQ/Network/Contacts.csv`:

```
ContactID,Name,Company,Title,LinkedIn,Email,Lane,Priority,Warmth,Source,FirstContact,LastTouch,NextTouch,IntervalDays,Owed,Notes
```

`HQ/Network/Interactions.csv`:

```
InteractionID,ContactID,Date,Channel,Direction,Summary,Signal,Outcome,NextAction,NextActionDate
```

`HQ/Tracker/Applications.csv`:

```
AppID,Company,Role,Status,DateApplied,Source,Location,WorkType,SponsorshipNeeded,ContactAtCompany,Stage,NextAction,NextActionDate,JobLink,Notes
```

---

## Step 4: Write the seven skills

Find the user's skills directory. In Claude Code that is `.claude/skills/` inside the project or workspace they will work in, or `~/.claude/skills/` for all projects. Ask which they want. If they are unsure, put it next to `HQ` and tell them plainly where it went.

For each skill below, create a folder named after the skill and write the content as `SKILL.md` inside it.

**In every one, replace `{{HQ}}` with the real absolute path from Step 0.**

**Write these files directly. Do not script the substitution.** On Windows the path contains backslashes, and `sed`, `perl` and most find-and-replace tools read those as escape characters. `C:\Users\Sam\Documents` silently becomes `C:SERSSAMDOCUMENTS`, the skill then points at a folder that does not exist, and nobody finds out until the first CV fails.

After writing them, check two things: that no `{{HQ}}` remains anywhere, and that the `HQ` line in each file reads back as the correct path with its backslashes intact.

### `tailor-cv/SKILL.md`

````markdown
---
name: tailor-cv
description: "Tailors the user's CV to one specific job description. Use whenever they paste a job description or job posting and ask to tailor, adapt, customise, rework or optimise their CV or resume for it, or say things like 'tailor my CV for this job', 'match my resume to this posting', 'make my CV fit this JD', 'ATS-optimise my CV', or name a company and role and ask for a CV. Reads their positioning, fact ledger and CV rules first, then produces a truthfully tailored, keyword-matched CV in Output/."
---

# Tailor the CV

Produce a CV for one specific job description, built only from things the user has actually done.

`HQ` = `{{HQ}}`

## Read first, every time

1. `HQ/Career_System/POSITIONING.md` - level, target lanes, skip list, tone.
2. `HQ/Career_System/CAREER_FACTS.md` - the fact ledger. **Nothing goes on the CV that is not traceable here or said by the user in this session.**
3. `HQ/Career_System/CV_RULES.md` - structure, the bullet framework, formatting, banned words.
4. The most recent CV in `HQ/Output/`, if one exists. That is the working template for structure and visual format.

## Workflow

**1. Get the job description.** If they pasted it, use it. If they only named a company and role, ask for the text or a link. Never infer requirements from a job title.

**2. Pull the posting apart.** List the hard skills and tools named, the responsibilities, the seniority signals, and the exact phrasing used for each. Screeners match strings. "Stakeholder management" and "cross-functional collaboration" are not interchangeable.

**3. Match honestly.** Each requirement lands in one of three buckets:

- **Direct match.** They have done it. Use the employer's own words where those words genuinely describe the same thing.
- **Adjacent.** Related but not identical. Describe what they actually did. Do not relabel it as the employer's term if that overstates it.
- **Gap.** No evidence in the ledger. Leave it out. Mention the significant ones in the reply so they can decide whether to handle it in the letter or at interview. Never paper over a gap with a vague claim.

**4. Decide the shape.** Follow CV_RULES.md. Experience leads for an experienced hire. Education leads only for a recent graduate or a graduate scheme. Real titles only, always. If a title is genuinely misleading about the work, add a plain function tag in brackets rather than changing it.

Include older roles in condensed form. They close date gaps and prove tenure.

**5. Draft the sections.**

- **Professional summary.** Two to four sentences. Open at their real level. Foreground the two or three things this posting cares about most. No adjective that could describe anyone.
- **Experience bullets.** Reorder so the most relevant lead. Rewording for keyword alignment is fine; changing what they did is not. Every bullet uses the framework in CV_RULES.md and opens with an action verb.
- **Projects.** Pick the two or three that answer this posting. Drop the rest.
- **Skills line.** Only what is genuinely true, checked against the skills table. Never upgrade a proficiency level. A skills line means "has used", not "expert in", unless the posting asks for a level.
- Keep education and additional information broadly stable, adjusting only what this posting makes relevant.

**6. Apply the voice rules** from CV_RULES.md. Check the banned list before finishing.

**7. Build the file.**

**Never read `word/document.xml` into context.** A formatted CV's XML runs to tens of thousands of tokens and costs more than the rest of this task combined. In order of preference:

- If a `docx` skill is available in this environment, use it.
- Otherwise, if a previous CV exists in `HQ/Output/`, copy it and write a short script that unpacks the file, does targeted find-and-replace on the text, and repacks it. The script touches the XML; you never load it. Confirm the result by opening it, not by reading the markup back.
- If neither is possible, produce clean Markdown and say plainly that they need to paste it into their own template.

Page limit from CV_RULES.md. Check it before delivering, do not guess.

**8. Save** as `HQ/Output/[Name]_CV_[Company]_[ShortRole].docx`, flat, no subfolder.

**9. Report back briefly.** Which requirements matched directly, which real gaps were left out, and the filename. Do not explain the tailoring line by line. They can read the CV.

## Hard rules

- Never invent a skill, metric, employer, title or achievement to close a keyword gap.
- Never claim years with a tool that do not match their timeline.
- Never claim anything listed under "things that are NOT true" in the fact ledger.
- Never state a salary figure.
- If the posting is far enough from their background that a truthful CV would look thin, say so plainly instead of stretching it. That is a favour, not a criticism.
- After the CV is built, offer once to log the application and find two people at the company worth contacting. One offer. If they decline, drop it.
````

### `cover-letter/SKILL.md`

````markdown
---
name: cover-letter
description: "Writes the user's cover letters. Use when they ask for a cover letter, covering letter, motivation letter or speculative letter for a role, say 'write the cover letter for this', 'draft a covering letter', 'I need a letter to go with this application', or ask to approach a company with no advertised vacancy. Handles both response letters answering an advert and speculative letters to a named manager."
---

# Cover letter

`HQ` = `{{HQ}}`

## Read first

1. `HQ/Career_System/POSITIONING.md`
2. `HQ/Career_System/CAREER_FACTS.md`
3. `HQ/Career_System/CV_RULES.md`, the cover letter section
4. The tailored CV for this role in `HQ/Output/`, if one exists. **The letter must not repeat its bullets.**

## Before drafting, establish three things

**Who it is addressed to.** Always try for a named person. Ask them to check the company site or LinkedIn for the hiring manager or team lead. "Dear Hiring Manager" is the fallback, not the default. For a speculative letter a named person is not optional, and it should not go to HR.

**What they actually know about the company.** Not what is on the homepage. Something researched: a product they shipped, a change hitting their customers, a funding round and what it is for, something a person there said. If there is nothing, say so and ask them to spend ten minutes finding one thing, or offer to search. A generic paragraph two is the reason most letters fail.

**Whether there is a connection.** A conversation, an event, a former colleague, an alum. If there is, it goes in the first line and it changes the whole letter.

## Structure

Follow the five-part structure in CV_RULES.md. One page. Same font as the CV. Formal letter layout.

## Voice

Peer to peer. They are an experienced person offering to solve a problem, not an applicant hoping to be let in. Understated. Follow the voice rules in CV_RULES.md and check the banned list.

First person is correct here. The no-pronouns rule applies to the CV, not the letter.

Never write a sentence they would not say out loud.

## Build

Use the `docx` skill if available. Otherwise copy the most recent letter in `HQ/Output/` and script the find-and-replace. **Never read `word/document.xml` into context** — it is enormous and it is the single most expensive thing you can do in this task. Confirm it fits one page.

Save as `HQ/Output/[Name]_CoverLetter_[Company]_[ShortRole].docx`.

## Hard rules

- Every claim traces to CAREER_FACTS.md.
- No salary figures.
- Do not restate the CV. The letter earns its place by carrying motivation, context and evidence the CV cannot.
- If there is nothing genuine to say about why this company, say so. A weak letter is worse than a short one, and worse than none where none is allowed.
- Address the standing objection from POSITIONING.md only when the posting makes it unavoidable. Otherwise hold it for interview.
````

### `outreach/SKILL.md`

````markdown
---
name: outreach
description: "Writes the user's networking and job search messages: cold emails to hiring managers, recruiter emails, LinkedIn connection notes and InMails, follow-ups, referral asks and thank yous. Use when they ask to write to a recruiter, message someone on LinkedIn, reach out to a hiring manager, ask for a coffee chat or a referral, follow up on silence, or say 'draft an email to', 'what do I say to', 'help me contact', 'nobody is replying' or 'my outreach is not landing'."
---

# Outreach

`HQ` = `{{HQ}}`

## Read first

1. `HQ/Career_System/MESSAGE_LIBRARY.md` - the templates and the three moves.
2. `HQ/Career_System/POSITIONING.md` - level, lanes, how salary and work rights are handled.
3. `HQ/Career_System/CAREER_FACTS.md` - **only the sections this message actually touches**, usually the current or most recent role. A 150-word email does not need the whole ledger loaded. Search it for what you need rather than reading it end to end.
4. `HQ/Network/Contacts.csv` - check whether this person already exists and what was said last time.

## Before writing anything, get one specific thing

Ask, or find: what does this person do, and what is one thing about their work that could only apply to them? Without it the message is a blast, and blasts are why outreach gets silence.

If they cannot supply it and it is an A-priority contact, spend the time finding it. If it is a C-priority contact, use the template with one line changed and move on. Effort follows priority.

## Choose the target before the template

Hiring managers, team leads and heads of function beat recruiters. They own the problem, they are not filtering CVs against a checklist, and an unusual background reads as interesting rather than as a mismatch. In-house talent acquisition sits in the middle. Agency recruiters are a volume channel, useful but secondary.

Direct email beats LinkedIn by a wide margin. If the company email format can be worked out, use it.

## Write it

Under 150 words. Under 120 is better. Three moves: context, connection, curiosity. Subject line of six words, specific, no hype.

Then check it against the voice rules in `HQ/Career_System/CV_RULES.md`. Read the first line as if it arrived from a stranger. **If it could have been sent to fifty people, rewrite it.**

## After drafting

- Show the draft. **Never send anything.** They send everything themselves.
- Attach the CV to recruiter emails only. Never attach anything to a first LinkedIn message.
- Never state a salary figure.
- Offer to add the person to `HQ/Network/Contacts.csv` and set the follow-up date. One offer, then drop it.

## When outreach is not landing

Diagnose using the list at the end of MESSAGE_LIBRARY.md and say which one it is, plainly. Usually it is target or volume, and people would rather hear it is the market.
````

### `network-crm/SKILL.md`

````markdown
---
name: network-crm
description: "Runs the user's networking CRM in Network/Contacts.csv and Network/Interactions.csv. Use when they ask who they should contact this week, who has gone quiet, who they owe a reply to, want to add someone to their network, log a message or a call, set or check a follow-up date, or ask for their weekly outreach list or a summary of the network. Also use after any outreach or networking call to record what happened."
---

# Network CRM

`HQ` = `{{HQ}}`

Two files:
- `HQ/Network/Contacts.csv` - one row per person, current state.
- `HQ/Network/Interactions.csv` - one row per contact made, append only.

The rules for warmth levels, intervals and priorities are in `HQ/Career_System/NETWORK_CADENCE.md`. Read it before making judgement calls. Today's date drives everything, so establish it before working out what is due.

## The four jobs

### 1. "Who should I contact this week?"

Read Contacts.csv. Anything with `NextTouch` on or before today is due. Sort by priority, then by how overdue it is. Present as a short table: name, company, why now, and what the message should be. Group by action type so the sending can be batched.

Cap the list at what can realistically be sent. If more is due than that, say what to drop and push the rest.

Then offer to draft the messages using the `outreach` skill.

### 2. "Add this person"

Get name, company and how they were found, at minimum. Fill in title, LinkedIn and email if available or findable. Assign:

- **Lane** from POSITIONING.md.
- **Priority** A, B or C, and say why.
- **Warmth** Cold.
- **NextTouch** within seven days. A cold contact who sits untouched for a month should be deleted rather than carried.

Write the row. Never overwrite an existing person. Check for duplicates by name and company first.

### 3. "Log this"

Append to Interactions.csv, then update the person's row in Contacts.csv: LastTouch, Warmth, NextTouch, IntervalDays, Owed.

The `Signal` column matters more than the summary. Capture the pain point, the tool complaint, the "we keep meaning to", in their own words. Those sentences are what makes the next message land, and what a cover letter to that company should open with.

Warmth transitions are in NETWORK_CADENCE.md. Apply them, do not improvise them.

### 4. "How is the network doing?"

Counts by warmth and by priority. Conversations booked in the last four weeks. Anyone in `Owed` with something outstanding, listed first, because those are reputation debts. Anyone Contacted for more than three weeks with no movement. New contacts added this week against the weekly target.

Say the honest number. If they added two people this week, say two.

## Rules

- Preserve CSV formatting exactly. Quote any field containing a comma. Never reorder columns. Never renumber IDs.
- Never invent a contact, an email address or an interaction that did not happen.
- **Never send anything.** Draft, show, let them send.
- Flag anything in `Owed` before anything else. Closing loops is the highest-value thing in the file.
- If nothing has been logged in two weeks, say so once, plainly, and offer to catch the log up from memory. Do not raise it again in the same session.
````

### `coffee-chat/SKILL.md`

````markdown
---
name: coffee-chat
description: "Prepares the user for a networking call or coffee chat and handles the follow-up afterwards. Use when they have a call booked with someone and ask to prepare, say 'I have a coffee chat with', 'what should I ask', 'prep me for this call', 'brief me on this person or company', or afterwards say 'that call went like this', 'log my chat with', or ask what to send as a thank you. Produces a one-page brief before, and a logged follow-up after."
---

# Coffee chat

`HQ` = `{{HQ}}`

A networking call is not an interview. The user runs it. Never prepare them to be interviewed.

## Job 1: the brief, before the call

Ask for the person's name, company and the meeting time if not given. Check `HQ/Network/Contacts.csv` for history.

Research, using web search where it helps, and produce a **one page brief**, no longer:

1. **The company in one sentence** a customer would recognise, plus what it actually sells.
2. **What changed in the last six months.** Funding, launches, leadership, layoffs, a shift hitting their customers.
3. **This person's path.** Where they were before, how long they have been there, whether they moved sideways into it.
4. **Anything they have written or said publicly.** Quote one line. This is the strongest possible opener.
5. **The opening line**, written out in full, twenty seconds spoken.
6. **Three questions**, not ten, matched to this person's role. Say why each is worth asking.
7. **The one link between their world and the user's experience**, held back until the last few minutes.

Flag anything that could not be verified. Never present a guess about a company as fact.

Keep prep to thirty minutes of their time. Hand over the brief and stop. Over-preparing is a way of avoiding the call.

## Good questions

Specific, cannot be answered from the website, and invite an opinion rather than a fact:

- How did you end up doing this?
- What does a normal week actually look like?
- What is the part of this job people underestimate?
- What is changing in this field that nobody outside it has noticed yet?
- If you were coming into this now, what would you do differently?
- Who else should I be talking to?

Never ask something answerable in ten seconds on their site. Never ask for a job.

## The close, which is not optional

Three things, every time:

1. Ask for a name. "Who else should I talk to?"
2. Ask permission to stay in touch.
3. End on time, or early. Ending early is remembered well.

## Job 2: the follow-up, after the call

When they report back, capture:

- The problem mentioned more than once.
- Any tool or process they complained about.
- Anything starting "we keep meaning to".
- Names they gave.
- Anything either side promised.

Then do three things:

1. **Log it.** Append to `HQ/Network/Interactions.csv` and update the person's row in `HQ/Network/Contacts.csv`. Warmth becomes Warm, or Advocate if they offered an introduction. LastTouch today, NextTouch per NETWORK_CADENCE.md, `Owed` filled in if anything is outstanding.
2. **Draft the thank you** using template 9 in `HQ/Career_System/MESSAGE_LIBRARY.md`. Within 24 hours. It must reference the single most useful thing they said and one action taken because of it.
3. **Act on the names.** Draft the introduction messages within the week, opening with "[Name] suggested I get in touch". A referred introduction goes cold fast.

## Rules

- No CV attachment, no job ask, no referral ask on a first call unless they raise it.
- If they are nervous, give them the opening line and the first question and say that is all they need. Do not pile on more prep.
````

### `apply-to-role/SKILL.md`

````markdown
---
name: apply-to-role
description: "Runs the user's full application sequence for one job in a single pass: tailored CV, cover letter if needed, tracker entry, and two people at the company worth contacting directly. Use when they paste a job description and say 'apply for this', 'do the whole thing', 'I want to go for this one', 'sort this application out', or ask what they need to send for a specific role. Do not use for CV-only or letter-only requests."
---

# Apply to a role

`HQ` = `{{HQ}}`

One job description in, a complete application out. Work through the steps in order and show each output as it lands, rather than disappearing and returning with everything at the end.

## Step 0: sanity check the role, in two lines

Against `HQ/Career_System/POSITIONING.md`: which lane is it, and is it on the skip list?

Check the things that waste time: a clearance, licence or certification they do not have; sponsorship they cannot get; a required domain they have no evidence in; a level well below where they are aiming.

If it is a poor fit, say so **before** doing the work and let them decide. They decide, not you. If they say go, go, and build it properly without sulking about it.

## Step 1: the CV

Run the `tailor-cv` skill. Full workflow, no shortcuts.

## Step 2: the cover letter

Only if the application asks for one, or if there is a gap the CV cannot answer and a letter can. Run the `cover-letter` skill.

If a letter is optional and there is nothing genuine to say about the company, say that a weak letter is worse than none, and let them choose.

## Step 3: the tracker

Add a row to `HQ/Tracker/Applications.csv`. Columns: AppID, Company, Role, Status, DateApplied, Source, Location, WorkType, SponsorshipNeeded, ContactAtCompany, Stage, NextAction, NextActionDate, JobLink, Notes.

Set `NextAction` to the outreach in step 4 and `NextActionDate` to two to three days after the application date.

## Step 4: two people at that company

This is the step that changes the odds, and the one everyone skips.

Find two named people: the hiring manager or team lead who owns this work, and one peer in the same function. **Not the recruiter.** Use LinkedIn, the company site, and the posting itself, which often names the reporting line.

For each, draft a short message with the `outreach` skill using template 2 in `HQ/Career_System/MESSAGE_LIBRARY.md`. Send two to three days after the portal application, not the same day.

Add both to `HQ/Network/Contacts.csv` through the `network-crm` skill, with NextTouch set to the send date.

## Step 5: the summary

Six lines maximum:

- What was produced and where it saved.
- The strongest genuine match between them and this role.
- The real gap, if there is one, and how to handle it if asked.
- Who to contact and when.
- Anything they need to supply before this goes out.

## Rules

- Every fact traces to `HQ/Career_System/CAREER_FACTS.md`.
- No salary figures anywhere.
- **Never submit anything, never send anything.** They do that.
- If they are doing several applications in one sitting, do them one at a time and finish each before starting the next. Half-finished applications are worse than fewer applications.
````

### `interview-prep/SKILL.md`

````markdown
---
name: interview-prep
description: "Prepares the user for a job interview and debriefs afterwards. Use when they have an interview booked and ask to prepare, say 'I have an interview at', 'help me prep', 'what will they ask me', 'practise with me', 'run a mock interview', or afterwards say 'the interview went like this' or ask what to send as a thank you. Produces a per-interview brief, rehearses the answers, and logs what was actually asked."
---

# Interview prep

`HQ` = `{{HQ}}`

## Read first

1. `HQ/Career_System/INTERVIEW_PLAYBOOK.md` - the story bank, the standing questions, the standing objection.
2. `HQ/Career_System/POSITIONING.md` - level, salary range, work rights.
3. `HQ/Career_System/CAREER_FACTS.md` - so nothing rehearsed is something that did not happen.
4. The tailored CV and cover letter for this role in `HQ/Output/`. **They will be asked about what is on the page.** Anything on the CV is fair game and must be defensible.

## Job 1: the brief

Get the company, role, interview format, who is on the panel and when it is. Then produce, in one page:

1. **The company in one sentence**, plus what it sells and to whom.
2. **What changed in the last six months.**
3. **The panel.** Background of each person, how long they have been there, what each will be assessing.
4. **Five likely questions**, specific to this posting, not generic.
5. **Which story from the bank answers each**, named, so they are not improvising.
6. **The hardest question this panel will ask**, and the answer in three sentences.
7. **Three questions to ask them.**

Flag anything unverified. Never present a guess about a company as fact.

## Job 2: rehearsal

Only if they want it. Ask.

Run it properly: ask one question, wait for the whole answer, then give feedback on three things and no more. Feedback that lists nine problems is not usable the day before an interview.

What to correct:

- **Waffle.** Two minutes maximum per behavioural answer. If they are still setting up the situation at forty seconds, cut it.
- **"We" instead of "I".** Interviewers need to know what this person did.
- **No result.** An answer that stops before the outcome is half an answer.
- **Over-explaining the objection.** Acknowledge, evidence, move on. Length signals worry.
- **Nothing to ask.** Never end with no questions.

Say what worked as well as what did not, and be specific about both. "That was good" teaches nothing.

## Job 3: the practicals

Two days before, cover: format and link or address, travel time, what to wear based on the company, whether anything needs preparing in advance, whether a task or presentation is expected, and the phone number to call if something goes wrong on the day.

For a presentation or task, confirm the time limit and practise it out loud, timed, at least twice.

## Job 4: the debrief

Same day. Capture every question asked, what went badly, and anything promised by either side.

Then:

1. Add the new questions to `HQ/Career_System/INTERVIEW_PLAYBOOK.md`. Each interview should make the next one easier.
2. Draft a short thank you to the person who ran it, within 24 hours, referencing something specific that was discussed.
3. Update the row in `HQ/Tracker/Applications.csv`: stage, next action, date.
4. If a story landed badly, rewrite it in the playbook now, while it is fresh.

## Rules

- Never rehearse a claim that is not in the fact ledger.
- Salary: deflect once, then give the range from POSITIONING.md. Never a single number, never below the floor.
- Never coach them to hide a gap. Coach them to state it in one sentence and move on.
- If the interview is tomorrow and they are anxious, cut the prep to the opening answer, three stories and three questions to ask. That is enough, and say so.
````

---

## Step 5: Hand over

Show them, short:

1. Where the folder is and what each file does.
2. The three sentences of their positioning, read back. **Ask them to correct it now.** Positioning written by someone else always needs one pass from the person it describes.
3. Anything marked `NOT YET CAPTURED` and what it would take to fill.
4. Exactly what to type next. Something like: paste a job description and say "apply for this".

Then stop. Do not tailor a CV in the same breath as setting the system up.

---

## Rules

- **Never invent a fact to fill a template.** An empty field is recoverable. A fabricated employer, metric or title is not, and it will surface in an interview.
- **Never push someone to inflate a title or a level.** Say what the risk is and let them decide.
- **Write the files above in full.** They are the system. A shortened CV_RULES.md produces worse CVs for the next two years.
- **Keep CAREER_FACTS.md tight.** It is read on almost every task, so every paragraph of waffle in it is paid for again and again. Facts, numbers and dates. No narrative.
- **Never read a .docx's internal XML into context.** Script the edit instead. It is the single most expensive mistake available in this system.
- Salary goes in POSITIONING.md and nowhere else. It never appears in a CV, letter or message.
- The user sends everything themselves. These skills draft, they never send, submit or apply.
- If they are mid-career and reluctant to talk about older roles, explain why the dates matter and get the two-line version.
- If they get tired partway through, stop and write what you have. The interview can resume next session, because the files persist.
