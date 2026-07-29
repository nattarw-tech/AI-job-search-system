# AI Job Search System

### Never forget, never fabricate.

Most people use AI for job hunting by pasting their CV into a chat and asking it to rewrite something. Two things go wrong.

**It forgets.** Close the chat and everything it learned about you is gone. Next time, you start again.

**It makes things up.** Ask it to match your CV to a job and it will invent a percentage, upgrade a job title, or claim a tool you have never opened. It sounds right, so you do not notice. Then someone asks about it in an interview.

This fixes both.

It interviews you once about your career and saves your answers to your own computer. After that, everything it writes comes only from those saved answers. Nothing invented, and nothing forgotten.

Then you paste a job advert, say **"apply for this"**, and get back a tailored CV, a cover letter, a tracker entry, and two people at that company worth emailing.

This system is free and always will be. It runs on your computer, and your details stay there. You will need a paid Claude plan to run it, but that money goes to Anthropic, not here.

---

## Before you start

**You need the Claude desktop app.** It is a normal app with a normal window. Download it at [claude.com/download](https://claude.com/download) and sign in. Mac, Windows and Linux.

**You need a paid Claude plan.** A free plan will run out partway through setup. That is not this system being greedy, it is just what AI assistants use.

**Set aside 45 minutes** for the setup interview, once. Have your current CV nearby if you have one. It makes things much faster.

You will not write any code. You type in plain English the whole way through.

> Already comfortable with a terminal, or use a different AI tool? See [Other ways to run this](#other-ways-to-run-this) at the bottom.

---

## Set it up

### 1. Download this project

Click the green **`<> Code`** button near the top of this page.

A small panel opens. If you see tabs called **Local** and **Codespaces**, click **Local**. Then click **Download ZIP**.

Now unzip the file. On Windows, right-click it and choose **Extract All**. On Mac, double-click it. Put the folder somewhere you will find again, like Documents.

The unzipped folder will be called **`AI-job-search-system-main`**, with `-main` on the end. That is normal — GitHub adds it to every download. Leave the name as it is.

### 2. Open the folder in Claude

Open the Claude app and click the **Code** tab at the top.

Click **Select folder** and choose the folder you just unzipped.

If it asks what kind of session you want, choose **Local**. That means "use the files on my own computer".

> **Windows users:** if the Code tab will not work, you need Git for Windows from [git-scm.com/downloads/win](https://git-scm.com/downloads/win). Install it and restart Claude. You will never use Git yourself — the app needs it underneath.

### 3. Type this

```
set up my job search system
```

That is the whole installation. It takes over from here.

---

## What happens next

First it asks where to keep your personal folder. **Choose somewhere outside this project folder**, like Documents. That keeps your private information separate.

Then it interviews you in six short rounds: where you are now, your work history, your skills and qualifications, your projects, what you are aiming for, and how you like to write.

Two things make the difference between this working well and working badly:

**Be specific.** "I improved a process" gives you a weak CV. "I cut invoice approval from nine days to four" gives you a strong one. If you are vague, it will ask you once for the real version. Let it.

**Be honest, including the awkward bits.** If you have a gap, say so. It will help you describe it calmly, which is much better than being caught out later.

You can stop halfway and come back another day. Anything you have already answered is saved.

---

## What you get

A folder of your own:

```
Job_Search_HQ/
  Career_System/     your facts, your targets, your writing style
  Network/           everyone you have contacted, and what was said
  Tracker/           every application in one place
  Output/            your finished CVs and letters
```

And these things you can ask for, in your own words:

| Say something like | You get |
| --- | --- |
| paste a job advert, then "apply for this" | The lot: CV, cover letter, tracker entry, two people to email |
| "tailor my CV for this" | One CV, matched to one advert |
| "write the cover letter" | A letter that adds to your CV instead of repeating it |
| "what do I say to this person?" | A short email or LinkedIn message |
| "who should I contact this week?" | A list from your contacts, with messages ready |
| "I have a coffee chat with Sam at Acme" | Notes before, a thank you after |
| "I have an interview on Thursday" | Likely questions, your answers, and a practice run |

Nothing to memorise. Ask for what you want and it works out the rest.

---

## The one rule

**Nothing goes into a document unless you said it.**

If a job advert asks for something you do not have, it tells you and leaves it out. You find out at your desk rather than in an interview.

It will also tell you when a job is a bad fit *before* doing the work, to save you the afternoon.

**It never sends anything.** Every email and application is written for you to read, change and send yourself.

---

## Making your plan go further

This is about **usage limits, not extra money**. Your plan lets you do a certain amount in a given period. Go over it and you wait for it to reset — you are not charged more. These habits mean you hit that limit far less often.

The reason is simple: each time you send a message, Claude re-reads the whole conversation so far. A long sprawling chat costs much more than several short ones.

**Start a new chat for each job.** This matters more than everything else here. If you do four applications in one conversation, the fourth one is still carrying the first three.

**Finish one application before starting the next.** Doing several at once feels efficient. It is the most wasteful way to work.

**Paste the job description, not the whole web page.** Menus, cookie banners and company boilerplate all count.

**Say what you want directly.** "Tailor my CV for this" uses less than a long conversation that gets to the same place.

The setup interview is the heaviest thing you will do, and you only do it once. Normal use afterwards is much lighter.

---

## If something goes wrong

**"It cannot find the instructions."**
It is looking at the wrong folder. Click **Select folder** again and choose the unzipped folder itself — the one with `README.md` inside it. Choosing the folder that *contains* it is the usual mistake.

**"It asked me something I do not know."**
Say "I do not know" or "skip that". It notes the gap and moves on.

**"It made something up."**
Tell it: "that is not in my facts file, take it out." Then check your `CAREER_FACTS.md` — usually the fact is simply missing, which is why it guessed. Add it and it will not happen again.

**"Can I change what it wrote about me?"**
Yes, and you should. These are ordinary text files. Open them and edit, or just tell Claude what to change. It is worth rewriting the file about your goals in your own words.

**"Do I have to do it all at once?"**
No. Stop whenever. Come back and say "carry on with my setup".

---

## What this does not do

- It does not apply for jobs. You send everything yourself.
- It does not find jobs. You bring the advert.
- It will not invent a better career than you have. It makes sure the one you have is presented properly.

---

## Your privacy

Everything stays on your computer. This project has no website, collects nothing and sends nothing anywhere.

What you type goes to Claude to be processed, exactly as in any normal conversation. That is between you and Anthropic, under their privacy policy. This project adds nothing to that.

Keep your `Job_Search_HQ` folder separate from this project folder. If you ever put a project online, you do not want your salary and work history going with it.

---

## Other ways to run this

**This was built for Claude Code, and that is the only setup I have tested.** Everything below is honest about what I know and what I do not.

### Terminal instead of the app

Same tool, different window. Install Claude Code from [claude.com/claude-code](https://claude.com/claude-code), then `cd` into the unzipped folder and run `claude`. Everything works identically.

### Other AI agents

Gemini CLI, OpenAI Codex, Cursor, Windsurf, Zed, Aider, GitHub Copilot and Manus Desktop can all read and write local files, and the instructions here are plain English, so they should be able to follow them. An `AGENTS.md` file is included, which those tools look for automatically.

**Two honest caveats.**

I have not tested any of them. If you try one, please open an issue and say how it went — that is genuinely useful and I will update this section.

More importantly, **you will lose the automatic part.** Claude Code recognises the seven skills on its own, so you just say "apply for this" and it knows what to do. Other tools do not read that folder. Your career files will be built correctly, but afterwards you will need to point the tool at the right instructions each time, like this:

```
Read job-search-setup/SKILL.md and follow the tailor-cv instructions for this job advert.
```

It still works. It is just more typing, every time.

### What will not work

**Browser chats.** ChatGPT, Gemini, Claude or Copilot in a web browser cannot save files to your computer, so nothing survives the conversation ending. That removes the entire point.

Note that ChatGPT in a browser and OpenAI's Codex are different products. Codex runs on your machine and can be used here. ChatGPT in a tab cannot.

**Manus cloud sandbox.** Manus running in the cloud keeps files in a temporary container rather than on your computer. Use Manus Desktop instead, which works locally.

---

## Contributing

Found something confusing or broken? Open an issue and say what happened. Feedback from people actually job hunting is the most useful kind.

Please do not submit your own career details as examples.

## Licence

MIT. Use it, change it, share it. No attribution required.
