# The Panaversity AI Method

The **Panaversity AI Method** is the way Panaversity's own team works with AI on every piece of real work, from a book chapter to a client report. It is also the way you work through every step of this bootcamp. The book describes it in [How the Panaversity team works](https://agentfactory.panaversity.org/claude-and-chatgpt-2/new-way-of-working/how-the-panaversity-team-works/#what-is-the-panaversity-ai-method). This page explains each of its five steps, and shows where each one happens in this bootcamp.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="../assets/panaversity-ai-method-dark.png">
  <img src="../assets/panaversity-ai-method-light.png" alt="The Panaversity AI Method: you define the work, AI does it, you decide when it is done. Five steps in a row. Step 1, define the problem: done by you. Step 2, set up the environment: done by you, with Claude. Step 3, write the four-part brief: done by you. Step 4, improve with the Dr. Gilsdorf method: done by Claude and a second AI, in rounds until 9.5. Step 5, check and commit: you decide." width="100%">
</picture>

One idea sits under all five steps: **AI does most of the work, and a person decides what the work is for and when it is done.** In this bootcamp, that person is you. In short, the work is human-directed, AI-executed, evidence-verified, human-approved and continuously improved.

## Contents

- [The five steps at a glance](#the-five-steps-at-a-glance)
- [Words you need](#words-you-need)
- [How much of the method to use](#how-much-of-the-method-to-use)
- [Step 1: Understand and define the problem](#step-1-understand-and-define-the-problem)
- [Step 2: Set up the environment](#step-2-set-up-the-environment)
- [Step 3: Write the four-part brief](#step-3-write-the-four-part-brief)
- [Step 4: Improve the work with the Dr. Gilsdorf method](#step-4-improve-the-work-with-the-dr-gilsdorf-method)
- [Step 5: Check and commit](#step-5-check-and-commit)
- [One bootcamp step, start to finish](#one-bootcamp-step-start-to-finish)
- [Rules that never change](#rules-that-never-change)
- [A prompt for anything you write](#a-prompt-for-anything-you-write)
- [Checklist before you tag a step](#checklist-before-you-tag-a-step)
- [References](#references)

## The five steps at a glance

| Step | What it means | Where you do it here |
| --- | --- | --- |
| **1. Understand and define the problem** | Decide what you want, why it matters and how you will know it is done. | Before you start a step, read Copperleaf's ask, **What you will make** and the **Submission checklist**: they are the problem and the "done" test. In the step 24 capstone, you define the problem yourself, from your own role. |
| **2. Set up the environment** | A safe place for the work that keeps every version, with Claude given only the access it needs. | Once, in [Step 00](../step-00-readiness-check/README.md), Part A, and [How we work](../README.md#how-we-work-local-first-human-in-the-loop) items 1 to 3: your fork, your local clone, a Claude project with the folder and the fork, and "never commit or push" in its instructions. Then a new thread for each step. |
| **3. Write the four-part brief** | Outcome, context, format and constraints, with the checks the work must pass. | Until step 12, each step's prompts under **Do it with Claude** are briefs written for you: read each one before you paste it, so you know what "done" means. From step 13 you change them to fit (each step's 🧭 note says how far), in [step 17](../step-17-four-part-brief/README.md) you learn the four parts, from step 21 you write them, and in the capstone you write one for a task from your own role. |
| **4. Improve the work with the Dr. Gilsdorf method** | Grade and improve the work in rounds toward 9.5 out of 10, run the checks, and get an independent review from a second AI. | You try it in [step 2](../step-02-three-deliverables/README.md) and do it in full in [step 4](../step-04-second-opinion/README.md). After that, use the [prompt below](#a-prompt-for-anything-you-write) on anything you write. The step's **Check it** section and checklist are the pass-or-fail checks. |
| **5. Check and commit** | A person checks the final result, approves it and saves it as the official version. | Each step's **Check it** and **Keep it** sections: check the facts against Copperleaf's files, open any Word or slide file the job made, read the changes in GitHub Desktop, then commit, tag `step-NN-done` and push them yourself, and submit as [SUBMITTING.md](../SUBMITTING.md) says. |

## Words you need

| Word | What it means |
| --- | --- |
| **Repo** (repository) | A project folder managed by Git, which records each saved version of its files |
| **Fork** | Your own copy of the bootcamp repo on GitHub, where all your work goes |
| **Clone** | Your copy of a repo on your computer |
| **Diff** | A view of exactly what changed: lines added in green, lines removed in red |
| **Commit** | A saved snapshot of your changes, with a short note saying what changed |
| **Push** | Sending your commits from your computer up to GitHub |
| **Tag** | A name on one commit, such as `step-04-done`, that marks a finished step for the grader |
| **Branch** | A separate line of work, so changes don't touch the main version until they are ready |
| **Claude project** | A workspace in Claude with its own files, instructions and threads (separate conversations) |
| **Markdown** | Plain text with simple marks, such as # for a heading, that shows as formatted text |
| **CSV** | Table data saved as plain text: one row per line, with commas between the columns |
| **Check** | A pass-or-fail test the work must pass, such as "every total matches Copperleaf's files" |

## How much of the method to use

Match the effort to the risk. A quick note doesn't need what a payment run needs.

| Level | Examples | How much of the method |
| --- | --- | --- |
| **Routine** | An email, notes, a question to Claude, brainstorming | A short brief, and a quick read before you use it |
| **Professional** | A report, a memo for a manager, any step of this bootcamp | All five steps, with pass-or-fail checks, an independent AI review and your approval |
| **High risk** | Payments, personal or client data, anything sent outside the company | All five steps, plus every figure checked by a person, and approval by someone allowed to approve it |

Copperleaf's money is made up, but treat its work as real: anything that decides a payment, a credit or a message to a customer is high risk, and a person always signs before it leaves the company.

## Step 1: Understand and define the problem

Know what problem you are solving, for whom, and how you will know it is solved, before you open Claude. If you can't say this in a few sentences, you aren't ready to hand the work to AI, and no prompt will fix that.

Answer four questions in plain words:

- **What is the problem, and why does it matter?** "Match this week's payments to open invoices, so Rosa knows which customers still owe money" says what and why. "Look at the payments" leaves Claude to guess.
- **Who is it for?** The person who will read, approve or use the result: here, someone at Copperleaf, such as Rosa, the finance manager.
- **What is in and out of scope?** The edges of the job, and the files it must work from in the `copperleaf/` folder.
- **What does done look like?** One "Done when" sentence that can be answered yes or no, or a number to match, such as "Done when every payment is matched or listed as a problem, and the totals agree with the bank file". "Done when it looks good" is neither.

**In this bootcamp:** each step's summary, `> 🍃 Copperleaf's ask`, **What you will make** and **Submission checklist** answer these four questions for you. Read them before you start. In the step 24 capstone, nobody answers them for you: you define a problem from your own role. The book calls this the [first 10 percent](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/first-10-percent/) of the work, and you study it in step 15.

## Step 2: Set up the environment

A good setup gives Claude everything it needs and gives you a record of every change, so nothing reaches your work unseen. Your work lives in a Git repo, your fork. Claude edits the files in your folder, and you commit them. If you ever use a cloud session, Claude may commit to its own separate branch there. Either way, no change Claude makes becomes part of your work until you approve it: that is the *human in the loop*.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="../assets/how-we-work-dark.png">
  <img src="../assets/how-we-work-light.png" alt="Your fork on GitHub is cloned to a folder on your computer with GitHub Desktop. A Claude thread does each step in that folder and saves its work. You read every change in GitHub Desktop, then commit, tag and push it to your fork, and submit. ChatGPT repeats the same job from attached files. The AI never commits or pushes." width="100%">
</picture>

You set it up once, in [Step 00](../step-00-readiness-check/README.md), Part A, following [How we work](../README.md#how-we-work-local-first-human-in-the-loop):

1. **Fork the bootcamp repo** on GitHub. Your fork is where all your work goes.
2. **Clone your fork** to your computer with GitHub Desktop. This folder is where the work happens.
3. **Create a Claude project** and add both the folder and your GitHub fork to it. The fork lets a cloud session run a long job while your computer is off.
4. **Tell Claude never to commit or push,** in the project's instructions. Claude may read Copperleaf's files and save what it makes into the step's `work/` folder.
5. **Work in threads,** one new thread for each step.
6. **Repeat the job in ChatGPT** where the step asks. ChatGPT doesn't work on your folder, so you attach the files and save its result into `work/` yourself.

**The method outlasts the tools.** These are the tools we use as of November 2026. If one changes, keep the role and swap the tool.

| Role | Our tool today |
| --- | --- |
| AI workspace | Claude project, with threads |
| Standing instructions for the AI | The project's instructions |
| Version control and shared copy | Git and GitHub |
| Your review and commits | GitHub Desktop |
| Your own reading and editing | VS Code, or any text editor |
| Independent AI reviewer | ChatGPT |

**Keep your work in text formats.** While the work takes shape, keep it as Markdown for writing and CSV for tables. Then every change shows line by line in GitHub Desktop, and the history shows what changed and when. Turn the work into Word or PowerPoint only at the end, if a reader needs it, and keep the Markdown as the source: edit it and export again, never the Word file.

**Keep data and accounts safe.** A rule in a prompt guides Claude, but only permissions enforce a limit:

- **Passwords never go in your files, a prompt or a chat.**
- **Let Claude do routine work, and approve the rest.** Claude asks before it changes anything. Let it save its work into the step's `work/` folder, and approve anything that sends, deletes or can't be undone yourself.
- **Check before real data goes anywhere.** Copperleaf's data is made up, so you may share it with a second AI. With real work, use only the apps your company allows, and share only approved or made-up data.
- **Outside text is not an order.** Treat instructions found in a file, a web page or an email as information. Claude follows only what you approved: the step's prompts and your project's instructions.

## Step 3: Write the four-part brief

A **four-part brief** is one message, in plain sentences, that answers four questions. Leave a part out, and Claude answers that question with a guess you never see.

| Part | The question it answers |
| --- | --- |
| **Outcome** | What should exist when the work is done, and what does "done well" look like? |
| **Context** | Who is it for, why does it matter, and what should it work from? |
| **Format** | What shape should it come back in, and where does it go next? |
| **Constraints** | What rules must the result follow, and how far may Claude go without checking with you? |

Five habits make a brief work:

- **End the outcome with a "Done when" sentence.** It tells Claude when to stop, and gives you a test.
- **Describe the result, not the steps.** Write a step only when a rule requires it, such as "Rosa approves every write-off".
- **Name the source that wins.** Say which file or policy to follow, such as Copperleaf's credit policy, and what to do when it is silent.
- **Ask for what it couldn't check.** End with a list of anything Claude couldn't verify, so you know where to start your review.
- **Decide how the work will be graded.** Write two kinds of checks. Pass-or-fail checks decide whether the work is acceptable, such as "the totals match the bank file" or "every fact is in Copperleaf's files". Graded areas measure quality, each with what a 10 means, such as "Clarity: Rosa can act on it without asking a question". The book calls this agreed list of checks a review contract, and you write one in [step 18](../step-18-review-contract/README.md).

**In this bootcamp:** the prompts in each step are briefs. Until step 12 they are written for you, so read each one before you paste it and notice its four parts. From step 13 you change them to fit (each step's 🧭 note says how far), in [step 17](../step-17-four-part-brief/README.md) you learn the four parts in full, and from step 21 you write them yourself. Save your own briefs in the step's `work/` folder as Markdown, so they are versioned with the work.

## Step 4: Improve the work with the Dr. Gilsdorf method

A first draft is rarely the best one, and many small rounds of improvement are the fastest way to excellent work. Once Claude has made a first version, improve it in small steps, over several rounds, until it reaches 9.5 out of 10 in each area. Iteration is the key. Grades measure quality, but the checks decide whether the work is acceptable: **a 9.8 never makes up for a wrong total.**

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="../assets/gilsdorf-method-dark.png">
  <img src="../assets/gilsdorf-method-light.png" alt="Start with your draft. Ask the best AI you have to run the checks, such as every figure matching its source, and grade the work out of 10. Improve it in one small step, then check and grade again, and repeat until every check passes and the grade reaches 9.5. Then give the work to a different AI for an independent review, without the first AI's grades, paste that review back into your first AI, fix what is right and run the checks again. You check the facts and read every change before you commit it. A failed check always outweighs a grade." width="100%">
</picture>

1. **Claude runs the checks and grades the work out of 10** in each area, with the best model your plan offers. Every grade cites its evidence, such as the file and row a figure came from.
2. **Claude improves it until each area reaches 9.5 and every check passes.** It improves a little, checks and grades again, and repeats. A grade goes up only when the work changed or new evidence came in.
3. **A different AI reviews it independently,** such as ChatGPT. Give it the brief, the checks, the source files and the work, but not Claude's grades, so it judges the work for itself. Ask for findings, each with the problem, its evidence, how serious it is and a fix.
4. **Paste the review back into Claude,** which weighs each finding, fixes the ones that hold up, and says why it rejected any others.
5. **Claude runs every check again on the final version,** because a fix can break something that was right before. Only then does the work go to Step 5.

Three habits keep the rounds honest:

- **Say what each grade means,** for example that accuracy means every figure can be found in Copperleaf's files.
- **Limit the rounds,** to three for example, so Claude improves the work and not just the score. At the limit, Claude stops and lists what it couldn't fix. A graded area below 9.5 can be accepted, with the gap written down. A failed check can't: a wrong figure is fixed before the work is kept.
- **Check what may go to another AI.** Each reviewer is one more company that sees the work. Copperleaf's data is made up, so it may go; with real work, follow your company's rules.

The grades are a guide, not proof: a 9.5 doesn't show that every fact is right, and two AIs agreeing doesn't either. That is why you check the facts yourself in Step 5. The method is named after Dr. Gilsdorf, who taught Zia Khan business communication in an MBA class at Arizona State University, and who taught that you improve what you write by going over it again and again.

## Step 5: Check and commit

AI can be confidently wrong, so the last word belongs to a person. You decide when the work is ready, and you take responsibility for it. Three words are easy to mix up: a **commit** saves a version of the work; **approval** is a person accepting the result; a **merge** or release makes it the official version. You work alone in your fork, so your commit after these checks is your approval.

1. **Check the facts against their sources.** Start with the list of anything Claude couldn't verify. Recompute a total or two yourself, as each step's **Check it** section shows.
2. **Review any problems still open** from the grades and the second AI's review, and decide on each one.
3. **Make the final formats a reader needs.** If Rosa needs a Word memo or a slide deck, have Claude make it from the Markdown, save it in `work/` beside its source, then open it as Rosa would and check that nothing was lost: tables, figures and page breaks.
4. **Read the diff in GitHub Desktop,** including new files. Keep or discard each change, so you know exactly what you are accepting.
5. **Commit by hand** with a message that says what changed. If anything changed after Claude's final checks, check those parts again first. Then tag the commit `step-NN-done` and push it to your fork, as each step's **Keep it** section shows.

**On a team** (at work, not in this bootcamp), your work goes on a separate branch, and the project owner reviews it in a pull request before it joins the main version. Never open a pull request to the bootcamp repo.

**Learn from each step.** After each step, take five minutes to ask what Claude got wrong more than once, what the brief was missing, and which check caught a real problem. Write the answers in the step's `NOTES.md`, and put lasting lessons in your Claude project's instructions, so the next step starts with them. Read those changes before you keep them, because they shape every later step.

## One bootcamp step, start to finish

Here is [step 1](../step-01-first-whole-job/README.md), the first whole job, through the five steps:

| Step | What you do |
| --- | --- |
| **1. Define** | Read Copperleaf's ask: Rosa spends every Monday matching payments to invoices. Done when every payment is matched or listed, and a one-page summary tells Rosa what to do. |
| **2. Set up** | Already done in Step 00. You start a new thread for step 1 in your Claude project. |
| **3. Brief** | You read and paste the brief in instruction 6: it names the outcome (a matches file and a one-page summary), Copperleaf's payment, invoice and customer files, the credit policy as the source that wins, and where to save the result. |
| **4. Improve** | You repeat the job in ChatGPT and compare the two results payment by payment: a second AI's independent view. From step 2 on, you add the full grading rounds. |
| **5. Check and commit** | You run **Check it** yourself: every payment there once, the total added up by you, five matches spot-checked. Then you read the diff, commit, tag `step-01-done` and push to your fork. |

## Rules that never change

- **Claude never commits or pushes.** You read every change in GitHub Desktop and commit it yourself. That is the human in the loop.
- **Claude asks before it acts.** Let it do routine work in the step's `work/` folder, and approve anything that sends, deletes or can't be undone yourself.
- **Checks outrank grades.** A grade is an opinion. A wrong figure fails the work, whatever the grade says, so you check the facts yourself.
- **Share only what is allowed.** Copperleaf's data is made up, so you may give it to a second AI. With real work, send another AI only what your company's rules allow.
- **Your work stays in your fork.** Never open a pull request to the bootcamp repo.

## A prompt for anything you write

Paste this into the step's thread when a deliverable is ready, before you commit it:

```text
Before I keep this, check every figure and fact in it against Copperleaf's files and list any that don't match. Then grade it out of 10 in three areas: accuracy, quality, and how easy it is for the reader to understand. Give the evidence for each grade. A wrong figure counts for more than any grade. Improve it in small rounds until every check passes and each area reaches 9.5, for at most three rounds, and then list anything still open and anything you couldn't check. Never commit or push.
```

Then give the work and its sources to a second AI, such as ChatGPT, and ask it to review and grade the same three areas, with specific fixes and evidence. Don't show it Claude's grades. Paste its review back into the thread and ask Claude to weigh each point, fix what is right, and check the facts again.

## Checklist before you tag a step

- [ ] You know the step's "Done when": what the finished work must show.
- [ ] You worked in a thread of your Claude project, and Claude didn't commit or push.
- [ ] Every check in **Check it** and the checklist passes on the final version.
- [ ] Each graded area reached 9.5, or you wrote down the gap.
- [ ] From step 2 on, a second AI reviewed the work without Claude's grades, and Claude weighed its findings.
- [ ] Any Word or slide file is made, opened and saved in `work/` beside its source.
- [ ] You read the whole diff, committed it by hand, tagged `step-NN-done` and pushed it to your fork.
- [ ] What this step taught you is in `NOTES.md`, ready for the next one.

## References

From [The AI Agent Factory](https://agentfactory.panaversity.org/), the book this bootcamp accompanies:

- [How the Panaversity team works](https://agentfactory.panaversity.org/claude-and-chatgpt-2/new-way-of-working/how-the-panaversity-team-works/): the full description of the method, with its diagrams.
  - ["What is the Panaversity AI Method?"](https://agentfactory.panaversity.org/claude-and-chatgpt-2/new-way-of-working/how-the-panaversity-team-works/#what-is-the-panaversity-ai-method): the five steps and when to use each.
  - ["Where does the work live?"](https://agentfactory.panaversity.org/claude-and-chatgpt-2/new-way-of-working/how-the-panaversity-team-works/#where-does-the-work-live): the repository, the Claude project and committing by hand.
  - ["How do we improve the work?"](https://agentfactory.panaversity.org/claude-and-chatgpt-2/new-way-of-working/how-the-panaversity-team-works/#how-do-we-improve-the-work): the Dr. Gilsdorf method, step by step.
- [The first 10 percent](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/first-10-percent/): defining the problem before the work starts.
- [The four parts](https://agentfactory.panaversity.org/managing-ai-workers/the-four-part-brief/four-parts/): the four-part brief in full.
- [Agree the checks](https://agentfactory.panaversity.org/managing-ai-workers/the-review-contract/agree-the-checks/): the review contract.
- [Appendix: versions and pull requests](https://agentfactory.panaversity.org/appendices/claude-and-chatgpt-2/appendix-versions-and-pull-requests/): why a person reads every change before it is kept.

---

[Back to the bootcamp README](../README.md#how-we-work-local-first-human-in-the-loop)
