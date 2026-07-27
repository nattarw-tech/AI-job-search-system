# AGENTS.md

This project is a personal job search system. It is not application code. There is nothing to build, install or test.

## What to do

If the user asks to set up a job search system, build a CV workflow, or anything similar:

**Read `.claude/skills/job-search-setup/SKILL.md` and follow it exactly.** That file contains the full setup process: a structured interview, the six career files to write, three CSV files, and seven task-specific instruction files to generate.

Do not improvise a shorter version. The file is long because the content it writes out is the product.

## After setup

The setup creates a folder (default `Job_Search_HQ`) containing the user's career facts, plus seven instruction files covering: tailoring a CV, cover letters, outreach messages, a networking CRM, networking call prep, running a full application, and interview preparation.

When the user later asks for any of those things, read the matching instruction file and follow it. They live wherever the setup installed them, usually alongside the user's folder or in their agent configuration directory.

## The rule that matters

**Nothing may appear in a CV, cover letter, message or interview answer unless it is traceable to the user's `CAREER_FACTS.md` or was said by the user in the current session.**

No invented metrics. No upgraded job titles. No claimed tools or qualifications. If a job description asks for something with no supporting evidence, report it as a gap and leave it out.

Never send, submit or post anything. Draft it, show the user, let them send it.

## Privacy

The user's career folder is private. Never commit it to version control, never include its contents in a pull request, and never transmit it anywhere.
