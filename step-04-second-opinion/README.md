# Step 04: A Second Opinion and the Human Check

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Work the way Nisha does in the book's first case. Claude drafts a Copperleaf memo for the bank and grades its own work in rounds against a goal you set, ChatGPT reviews it as a second opinion, and you check every fact against Copperleaf's files before it is used. You see what each reviewer catches, and why the last check is always a person's.

> 🍃 **Copperleaf's ask:** Copperleaf's bank wants a one-page summary of what customers owe before it renews the overdraft. Rosa wants it checked by more than one pair of eyes, and she will sign it only if every figure is right.

> ⏱️ **About 5 to 6 hours**, including the reading. Good places to pause: after instruction 2, after instruction 5, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later. Each round is a good stopping point too, because `rounds.md` keeps the history.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [Case 1: Nisha's AI Team](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-1-nishas-ai-team/overview/): the case this step follows.
- [Steps 1 to 3: Claude writes and grades its own work](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-1-nishas-ai-team/steps-1-to-3-claude-writes-and-grades-its-own-work/): draft, grade and improve in rounds.
- [Steps 4 to 6: a second opinion and the human check](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-1-nishas-ai-team/steps-4-to-6-a-second-opinion-and-the-human-check/): ChatGPT as the second reviewer, and you as the last check.
- [How the Panaversity team works, "How do you keep the rounds honest?"](https://agentfactory.panaversity.org/claude-and-chatgpt-2/new-way-of-working/how-the-panaversity-team-works/#how-do-you-keep-the-rounds-honest): what each grade means, and limiting the rounds.
- [Questions for discussion](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-1-nishas-ai-team/questions-for-discussion/): the questions you answer in your notes.
- [Lab: take Nisha's method to 2.0](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-1-nishas-ai-team/lab-take-nishas-method-to-2-0/): the book's version of this step. The Copperleaf job below replaces it; doing both is optional extra practice.
- [Exhibits](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-1-nishas-ai-team/exhibits/): the case's documents, to compare with what you make.
- [Check yourself](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-1-nishas-ai-team/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

An AI can grade its own work, and each round usually makes the writing better. But a writer grading itself tends to miss its own blind spots, and better writing is not the same as true writing. Nisha's method adds two more pairs of eyes: a **second opinion** from a different AI, which notices different things, and a **human check** of every fact, which is the only check that can say "this figure is right" and mean it.

A summary for a bank is exactly where this matters. A wrong figure there is not a typo: it is a false statement to a lender, signed by Rosa.

## What you will learn

- How to set a goal and a grading guide before the AI writes, so a grade means something.
- How to run rounds of draft, grade and improve, and when to stop.
- What a second opinion from another app adds, and what it can't do.
- How to fact-check a document line by line against its sources.

## What you will make

- `work/goal.md`: the goal and grading guide, written before the first draft
- `work/bank-summary.md`: the final one-page summary
- `work/rounds.md`: each round's grade and what changed
- `work/chatgpt-review.md`: ChatGPT's second opinion, and what you did with each point
- `work/fact-check.md`: every figure and claim in the summary, its source, and whether you confirmed it
- `NOTES.md`: your answers to the case's discussion questions, and what each reviewer caught

## Key concepts

- **Goal:** what a finished piece of work must achieve, written before the work starts, so it can be graded.
- **Round:** one cycle of draft, grade against the goal, and improve.
- **Writer and reviewer:** two separate threads, one that writes and one that only grades, so the grader isn't marking its own work as it writes.
- **Second opinion:** a review by a different AI, which tends to catch different mistakes.
- **Human check:** a person confirming each fact against its source before the work is used. It is never skipped.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync and start the writer thread.** Sync your fork and pull in GitHub Desktop. Start a new thread for this step and call it `Step 04 writer` ([Finding things in the apps](../step-00-readiness-check/README.md#a-thread-in-your-project-and-its-name) shows how to rename a thread).

This step is the [Dr. Gilsdorf method](../step-02-three-deliverables/README.md#do-it-with-claude) from step 2 ([How the Panaversity team works](https://agentfactory.panaversity.org/claude-and-chatgpt-2/new-way-of-working/how-the-panaversity-team-works/#how-do-we-improve-the-work) in the book), done properly: a goal and grading guide written first, a separate reviewer thread that grades each round, and a second AI (ChatGPT) for the independent review at the end. Each round's grade goes in `work/rounds.md`.

**2. Write the goal first.** Paste:

```text
I'm doing Step 04 of the bootcamp. Before any drafting, help me write step-04-second-opinion/work/goal.md: the goal and grading guide for a one-page summary of what Copperleaf's customers owe, for its bank, as of Monday 2 November 2026.

The summary must: give the total owed and how much is overdue, by age band; name the largest single exposure; say what the credit policy does about late accounts; be true to the figures in step-02-three-deliverables/work/claude/figures.csv and the policy in copperleaf/policies/credit-and-collections-policy.md; and contain nothing a bank would need explained.

Write the guide as five criteria, each graded 1 (not yet), 2 (meets) or 3 (exceeds), with what each grade means. Show it to me before saving. Don't change anything else. Never commit or push.
```

Read the guide. Change anything that doesn't match what Rosa and the bank need, then reply `Save it`.

**3. Draft, round 1.** Paste:

```text
Draft step-04-second-opinion/work/bank-summary.md against work/goal.md, using only figures.csv and the policy. Put a short "Sources" line at the end naming the files. Then stop: don't grade it in this thread.
```

**4. Start the reviewer thread.** Start a second thread, `Step 04 reviewer`, and paste:

```text
You are the reviewer for Step 04. Read step-04-second-opinion/work/goal.md and step-04-second-opinion/work/bank-summary.md. Grade the summary on each criterion (1, 2 or 3), quoting the line that earns or loses each grade, and list the three changes that would most improve it. Check every figure you can against step-02-three-deliverables/work/claude/figures.csv. Write your grades into step-04-second-opinion/work/rounds.md under "Round 1". Don't edit the summary. Never commit or push.
```

**5. Improve, and stop after three rounds.** Go back to the writer thread and paste:

```text
Read work/rounds.md, round 1, and improve the summary. Change only what the review asks.
```

Then ask the reviewer for round 2 (`Grade it again under "Round 2".`). Stop when every criterion is at least 2, or after three rounds, whichever comes first. More rounds tend to polish the writing, not fix the facts.

## Repeat it in ChatGPT

In this step, ChatGPT plays a different role: it is the **second opinion**.

1. **Best: Codex on the same folder.** If you have Codex, OpenAI's agent app, open your `learn-ai-at-work` folder in it, so it reads `work/goal.md`, `work/bank-summary.md`, `step-02-three-deliverables/work/claude/figures.csv` and the policy exactly as they are, and add to the prompt below: `Review only. Don't change any files.` **Otherwise:** in your ChatGPT project (or, without one, a new chat), attach those four files, or a zip of them that you ask Claude to make.
2. Paste:

```text
You are a second reviewer, independent of the AI that wrote and graded this. Read goal.md and bank-summary.md. List anything that is wrong, unclear, missing or not supported by figures.csv or the policy. For each point, quote the line, say what is wrong and how sure you are. Don't rewrite the summary.
```

3. Save its answer as `work/chatgpt-review.md`. Under each point, add one line: *accepted*, *rejected* (and why) or *checked, not a problem*.
4. Give the accepted points to the writer thread in Claude and ask it to make only those changes.

With only one app, write a transfer plan in `NOTES.md` instead, and use a fresh Claude thread that has never seen the summary as your second reviewer. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

This is the human check. It comes last, and nobody else can do it.

- [ ] **Make the fact-check list.** Copy every figure and every policy claim in the final summary into `work/fact-check.md`, one per line.
- [ ] **Trace every figure.** For each figure, write where it comes from (`figures.csv`, a band total, a customer total) and confirm it yourself. Add up at least the total owed and the overdue total in your spreadsheet.
- [ ] **Trace every policy claim.** Open the policy at the section and confirm it says that.
- [ ] **The largest exposure is right.** Find the customer with the largest balance in `figures.csv` yourself, and compare it with its limit in `customers.csv`.
- [ ] **Nothing extra.** No figure or claim in the summary that you couldn't trace. Remove or fix any that you couldn't.
- [ ] **Mark it.** At the end of `work/fact-check.md`, write "Checked by <your name>, <date>". Only now could Rosa sign.

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-04: bank summary with a second opinion` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-04-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/goal.md`, written before the first draft (your commit history may show it; it doesn't have to yet)
- [ ] `work/bank-summary.md` and `work/rounds.md`, with no more than three rounds
- [ ] `work/chatgpt-review.md`, each point marked accepted, rejected or checked (or a transfer plan in `NOTES.md`)
- [ ] `work/fact-check.md`, with every figure and claim traced
- [ ] **Checked:** every figure and policy claim in the summary traced to its source by you
- [ ] `NOTES.md`: your answers to the case's [questions for discussion](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-1-nishas-ai-team/questions-for-discussion/), and one thing each reviewer (Claude, ChatGPT, you) caught that the others didn't
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] Committed, tagged `step-04-done` and pushed

## References

- [Case 1: Nisha's AI Team](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-1-nishas-ai-team/overview/)
- [How the Panaversity team works](https://agentfactory.panaversity.org/claude-and-chatgpt-2/new-way-of-working/how-the-panaversity-team-works/)
- Copperleaf's [customer list](../copperleaf/customers.csv) and [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md)

---

[← Step 03: Behind the Screen: A Safe Desk for the Work](../step-03-behind-the-screen/) · [Roadmap](../README.md#roadmap) · [Step 05: An Overnight Job for a Client →](../step-05-overnight-client-job/)
