# AI Job Search System

Most people use AI for job hunting by pasting their CV into a chat window and asking it to rewrite something. It works once. Then the chat closes, everything it learned about you is gone, and next time you start over.

Worse, it makes things up. Ask an AI to match your CV to a job and it will quietly invent a percentage, upgrade a job title, or claim a tool you have never opened. You do not notice, because it sounds right. Then someone asks about it in an interview.

This fixes both problems.

It interviews you once about your career, writes what you tell it into a set of files on your own computer, and then uses only those files to build everything afterwards. Nothing gets invented, because there is a written record of what is true and everything traces back to it. And it remembers, because the files stay on your machine between sessions.

After setup, you paste a job advert and say "apply for this". You get back a CV tailored to that advert, a cover letter, a row in your application tracker, and the names of two people at that company worth emailing directly.

**It is free, it runs on your own computer, and your career information never goes anywhere you did not send it.**

---

## What you need

**1. An AI tool that can read and write files on your computer.**

This is the only real requirement, and it rules out the ordinary chat websites. ChatGPT in a browser, Gemini in a browser and Claude in a browser cannot save files to your computer, so they cannot remember anything between conversations. You need what is usually called a "coding agent" or "CLI" — it runs on your machine and can open and save files.

The easiest one is **Claude Code**. Installation instructions are at [claude.com/claude-code](https://claude.com/claude-code). You need a Claude account.

**Expect to need a paid subscription.** A 45-minute setup interview followed by regular CV builds is more than free tiers are designed to carry, on any of the major providers. You will probably hit a limit partway through setup on a free plan. That is not a flaw in this system, it is what running an AI agent costs. See [Keeping the cost down](#keeping-the-cost-down) for how to make a subscription stretch.

If you run a model locally on your own hardware, cost stops being a factor, though you will need a capable machine and a model good enough to follow long instructions accurately.

Other tools work too. See [Using a different AI tool](#using-a-different-ai-tool) below.

**2. About 45 minutes**, once, for the setup interview.

**3. Your current CV**, if you have one. Not essential, but it makes the interview much faster.

You do not need to know how to code. You will not write any code. You type in plain English throughout.

---

## Setting it up

### Step 1: Download this project

Click the green **Code** button at the top of this page.

A small panel opens. Depending on your account, it may show tabs along the top — **Local** and **Codespaces**. **Make sure you are on the Local tab.** If you land on Codespaces you will not see the download option at all, which is the usual reason people get stuck here.

On the Local tab, click **Download ZIP** at the bottom.

Then unzip it somewhere you will find again, like your Documents folder. On Windows, right-click the downloaded file and choose **Extract All**. On Mac, double-click it.

If you know how to use Git, clone it instead. If you do not know what that means, ignore this line — the ZIP is fine.

### Step 2: Open your AI tool in that folder

Install Claude Code if you have not already, following the instructions on its website.

Then open a terminal — that is the black window where you type commands. On Windows it is called Terminal or PowerShell; on Mac it is called Terminal. Search your machine for it by name.

Type this, replacing the path with wherever you unzipped the folder:

```
cd "C:\Users\yourname\Documents\ai-job-search-system"
```

Then type:

```
claude
```

That starts Claude Code inside the project folder, which is how it finds the setup instructions.

### Step 3: Say the words

Type this and press enter:

```
set up my job search system
```

That is the whole installation. It takes over from here.

---

## What happens next

It asks where you want your personal folder to live. **Put it somewhere outside this project folder** — your Documents folder is ideal. That keeps your private career information separate from the downloaded project.

Then it interviews you, in six short rounds:

1. **Where you are now** — location, whether you can work in the countries you are targeting, how many years you have been working
2. **Your work history** — every job, what you actually did, what changed because of you
3. **Skills, tools, qualifications** — with honest levels, not inflated ones
4. **Projects and anything outside work** that shows what you can do
5. **What you are aiming for** — target roles, what you will refuse, your salary range
6. **How you write** — British or American English, words you never want used in your name

Answer honestly, including the awkward parts. If there is a gap in your CV, say so — it will help you describe it calmly, which is far better than being caught out later.

**Be specific.** This is the single thing that decides whether the system is any good. "I improved a process" produces a weak CV. "I cut invoice approval from nine days to four" produces a strong one. If you are vague, it will push you once for the real version. Let it.

You can stop halfway through and come back another day. Everything answered so far is already saved.

---

## What you end up with

A folder on your computer, yours, private:

```
Job_Search_HQ/
  Career_System/
    POSITIONING.md          what you are going for, and what you are not
    CAREER_FACTS.md         every job, achievement, tool and qualification
    CV_RULES.md             how your documents get written
    MESSAGE_LIBRARY.md      templates for emails and LinkedIn messages
    NETWORK_CADENCE.md      who to contact, and how often
    INTERVIEW_PLAYBOOK.md   your stories, and the questions you will be asked
  Network/                  everyone you have contacted, and what was said
  Tracker/                  every application, in one file
  Output/                   your finished CVs, letters and briefs
  Source_Material/          your old CV and anything else
```

Plus seven abilities you can use just by asking in plain English:

| Say this | You get |
| --- | --- |
| paste a job advert, then "apply for this" | The whole thing: CV, cover letter, tracker entry, two people to email |
| "tailor my CV for this" | One CV, matched to one advert, nothing invented |
| "write the cover letter" | A letter that adds to your CV instead of repeating it |
| "what do I say to this person?" | A short cold email or LinkedIn message |
| "who should I contact this week?" | A ranked list from your contacts, with drafts ready |
| "I have a coffee chat with Sam at Acme" | A one-page brief before, a thank you note after |
| "I have an interview at Acme on Thursday" | Likely questions, your best answers, and a practice run |

You do not memorise these. Ask for what you want in your own words and it works out which one applies.

---

## The rule the whole thing runs on

**Nothing goes into a document unless you said it.**

Not "probably true". Not "close enough". If a job advert asks for something you do not have, the system tells you it is a gap and leaves it out, so you find out sitting at your desk instead of in an interview.

It will also tell you when a job is a bad fit **before** doing the work, rather than producing a hopeful application. That is deliberate. It is trying to save you the afternoon.

**It never sends anything.** Every email, message and application is written for you to read, change and send yourself. Nothing goes out without you pressing the button.

---

## Using a different AI tool

The system is just a set of written instructions, so any capable AI can follow them. The only hard requirement is that it can read and write files on your computer.

**Claude Code** is the smoothest, because it recognises the instructions automatically. Nothing to configure.

**Other agent tools** — Gemini CLI, OpenAI Codex, Cursor, GitHub Copilot, Windsurf, Zed, Aider, JetBrains Junie and others — read a file called `AGENTS.md`, which is included here. Open your tool in this folder and say "set up my job search system". It should find its way. If it does not, tell it to read `.claude/skills/job-search-setup/SKILL.md` and follow it.

**Browser chat tools** — ChatGPT, Gemini and Claude on the web — will not work properly. They cannot save files to your computer, so nothing survives the conversation ending, which removes the entire point. You can paste the instructions in and get one CV out of it, but you will be starting from scratch every time.

---

## Keeping the cost down

AI tools charge by how much text they read and write. Every message you send re-sends the whole conversation so far, so a long rambling session costs far more than several short focused ones. Five habits do most of the work:

**1. Start a fresh conversation for each job.** This is the big one. In Claude Code, type `/clear` between applications. Otherwise application number four is still carrying applications one, two and three in memory, and paying for them every time.

**2. Do one application at a time.** Finish it, clear, start the next. Batching feels efficient and is the most expensive way to work.

**3. Keep `CAREER_FACTS.md` tight.** It gets read on nearly every task, so it is the file you pay for most often. Facts, numbers and dates. Not stories.

**4. Do not paste a whole careers page.** Paste the job description text. The navigation menu, the cookie banner and the company boilerplate all cost the same as the useful part.

**5. Ask for what you want.** "Tailor my CV for this" is cheaper than a conversation that wanders toward the same place.

The setup interview is the most expensive single session you will have, and it happens once. Day-to-day use afterwards is much lighter, because only the one instruction file needed for the task gets loaded rather than the whole system.

If you want to see what you are spending, Claude Code has a `/cost` command.

---

## Common problems

**"It says it cannot find the instructions."**
You are probably running it from the wrong folder. Close it, `cd` into the unzipped project folder, and start again. The instructions live inside the project, so it has to be started there.

**"It asked me a question I do not know the answer to."**
Say so. "I do not know" and "skip that" both work. It marks the gap and moves on.

**"It made something up anyway."**
Tell it. Something like "that number is not in my facts file, take it out". Then check `CAREER_FACTS.md` — usually the fact is missing from the file, which is why it improvised. Add it and it will not happen again.

**"Can I change what it wrote about me?"**
Yes, and you should. The files are ordinary text files. Open them in any text editor and edit freely, or just tell the AI what to change. `POSITIONING.md` in particular is worth rewriting in your own words — it was written about you by something that met you an hour ago.

**"Do I have to do the whole interview at once?"**
No. Stop whenever. Come back and say "carry on with my setup".

---

## What this does not do

- It does not apply to jobs for you. You send everything yourself.
- It does not find jobs. You bring the advert.
- It does not work without a tool that can access your files.
- It will not write you a CV that is better than your actual career. It will make sure your actual career is presented properly, which is a different and more useful thing.

---

## Your privacy

Everything lives on your own computer, in your own folder. This project has no server, collects nothing, and sends nothing anywhere.

The one thing to understand: whatever you type into your AI tool goes to that company's model to be processed, exactly as it would in any normal conversation with it. That is between you and them, and their privacy policy applies. This project adds nothing on top and takes nothing out.

If you keep your personal folder inside a project you later put on the internet, you could publish your own career details by accident. Keep `Job_Search_HQ` somewhere separate, like your Documents folder. A `.gitignore` file here tries to prevent this, but do not rely on it.

---

## Contributing

Improvements are welcome, particularly from people who have actually run a search with it. Open an issue describing what did not work.

Please do not open pull requests containing your own career information as examples.

## Licence

MIT. Use it, change it, share it, build on it commercially. No attribution required, though it is appreciated.
