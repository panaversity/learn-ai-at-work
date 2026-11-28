# Step 11: AI Fluency: The 4Ds

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Practise the four skills of working with AI: Delegation, Description, Discernment and Diligence. Before you hand over Copperleaf's weekly reminder job, you write a 4D plan for it: what to delegate, how to describe it, how you will judge the result, and what you stay responsible for. Then you run the job and compare what happened with your plan.

> 🍃 **Copperleaf's ask:** Ben wants to hand the weekly reminder list to an AI. Rosa says yes, but only after she has seen a plan for how it will be done and checked.

> ⏱️ **About 4 to 5 hours**, including the reading. Good places to pause: after instruction 4, after instruction 7, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [0.3.1 Three ways to work with AI](https://agentfactory.panaversity.org/how-ai-works/ai-fluency/three-ways/): automation, augmentation and agency.
- [0.3.2 The four Ds](https://agentfactory.panaversity.org/how-ai-works/ai-fluency/the-four-ds/): the four skills behind every step after this one.
- [0.3.3 Putting the 4Ds together](https://agentfactory.panaversity.org/how-ai-works/ai-fluency/putting-them-together/): using all four on one job.
- [Lab 0.3: Your 4D plan, before the run](https://agentfactory.panaversity.org/how-ai-works/ai-fluency/lab/): the book's version of this step. The Copperleaf version below replaces it.
- [Check yourself](https://agentfactory.panaversity.org/how-ai-works/ai-fluency/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

The AI Fluency Framework names four skills: **Delegation** (what the AI may do, and what waits for a person), **Description** (what it hands back, and how), **Discernment** (who checks the result, when, and against what) and **Diligence** (what may go in, who is told AI was involved, and who signs). In a chat, you do them as you go. When the AI works alone, there is no "as you go": every D must be decided **before the first run**, because nobody is there to decide it during the run.

Ben's reminder list is exactly that kind of job. A 4D plan, written first, is what Rosa is asking for. It is also the seed of almost everything in Part II: the brief, the review contract, the limits and the sign-off.

## What you will learn

- The three ways of working with AI (automation, augmentation and agency), and how to tell them apart.
- The four Ds, and when each is done when the AI works alone.
- How to write a 4D plan before a run.
- How to test one line of the plan, and compare the run with the plan.

## What you will make

- `work/4d-plan.md`, written and committed **before** the run
- `work/reminder-list.md`: the reminder list from the run
- `work/plan-vs-run.md`: what the run did against each line of the plan, and what you would change
- `NOTES.md`: how you sorted the three jobs, the Description test, and how the two apps compared

## Key concepts

- **Automation, augmentation, agency:** the AI does a task you describe; you and the AI think together; the AI works alone on tasks still to come.
- **Delegation:** deciding what the AI may do alone, and what waits for a person.
- **Description:** saying what the AI hands back, in what form, and what it does when something is missing.
- **Discernment:** judging the result: who checks it, when, and against what.
- **Diligence:** taking responsibility: what may go in, who is told AI was involved, and who signs.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync and start a thread.** Sync your fork, pull in GitHub Desktop, and start a new thread for this step.

**2. Sort three jobs.** Paste:

```text
I'm doing Step 11 of the bootcamp. Quiz me, one at a time, on which way of working each of these Copperleaf jobs is: automation (the AI does a specific task I describe), augmentation (we think it through together) or agency (the AI works alone, on tasks still to come). After each answer, tell me in one line whether I'm right and why.
1. "Turn this list of payments into a table sorted by amount."
2. "Help me work out why Harbourline's balance doesn't match their statement." We go back and forth.
3. "Every Monday morning, make the list of payment reminders due this week and leave it for Ben." Nobody watches it run.
```

Note your answers in `NOTES.md`.

**3. Write the 4D plan, before the run.** Paste:

```text
Help me write a 4D plan for job 3: every Monday morning, an AI makes the list of payment reminders due that week for Copperleaf, from the latest checked figures and copperleaf/policies/credit-and-collections-policy.md section 5, and leaves it for Ben. Nobody watches it run.

Ask me about one D at a time, and wait for my answer:
- Delegation: what may the AI do alone, and what waits for a person?
- Description: what does it hand back, in what form, and what does it do when the figures don't show something, such as a due date, or an invoice is disputed?
- Discernment: who checks the list, when, and against what?
- Diligence: what data may go in, who is told an AI made the list, and who signs before any reminder is sent?
For each D, also ask when it is done: before the first run, after each run, or throughout. Use my words and add no lines of your own. Then save the plan as step-11-ai-fluency/work/4d-plan.md, a table with the columns D, Line and When. Never commit or push.
```

Answer each question in your own words.

**4. Commit the plan before the run.** In GitHub Desktop, commit `work/4d-plan.md` on its own, with the summary `step-11: 4D plan, before the run`, and push. Its date in your history now comes before the run's.

**5. Test the Description line.** Open an incognito chat in Claude (the ghost icon at the top of a new chat; see [Finding things in the apps](../step-00-readiness-check/README.md#a-chat-that-keeps-nothing-incognito-or-temporary)) so memory can't help, attach `step-02-three-deliverables/work/claude/figures.csv` and the policy, and paste your plan's Description line followed by:

```text
Which invoices need a reminder this week, as of Monday 2 November 2026, and at which stage of the policy's section 5.1?
```

Then do the same in a second incognito chat **without** your Description line. Compare the two answers in `NOTES.md`: what did the line change?

**6. Run the job.** Back in your project thread, paste:

```text
Do the job in step-11-ai-fluency/work/4d-plan.md exactly as the plan describes, as of Monday 2 November 2026, using step-02-three-deliverables/work/claude/figures.csv and the policy. Save the list as step-11-ai-fluency/work/reminder-list.md. Draft only: send nothing. At the top, say which files you used. Never commit or push.
```

**7. Compare the run with the plan.** Do [Check it](#check-it), then paste:

```text
Make step-11-ai-fluency/work/plan-vs-run.md: one row per line of the 4D plan, with what the run actually did for that line. Leave a column "Kept?" and a column "What I'd change" for me to fill in.
```

Fill in the two columns yourself.

## Repeat it in ChatGPT

1. Do instruction 5's Description test in ChatGPT too, using a Temporary Chat (so memory can't help), with and without the line.
2. In your ChatGPT project (or, without one, a new chat with the same files attached), attach `work/4d-plan.md`, `figures.csv` and the policy, and run the job with the prompt from instruction 6. Save its list as `work/chatgpt-reminder-list.md`.
3. Check it the same way, and in `NOTES.md` compare it with Claude's list, line by line of the plan.

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **The plan came first.** In GitHub Desktop's **History**, the commit with `4d-plan.md` is earlier than the one with `reminder-list.md`.
- [ ] **Every D has a "when".** No line of the plan is missing it.
- [ ] **Delegation keeps sending with a person.** The plan says the AI drafts only, and a person signs (policy 5.3).
- [ ] **The list is right.** Check three reminders' stages yourself against section 5.1, and confirm no disputed invoice is on the list (6.2).
- [ ] **The run kept to the plan.** `plan-vs-run.md` is filled in by you, line by line.

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-11: run and comparison` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-11-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/4d-plan.md`, committed before the run
- [ ] `work/reminder-list.md` and `work/plan-vs-run.md`
- [ ] `work/chatgpt-reminder-list.md` (or a transfer plan in `NOTES.md`)
- [ ] **Checked:** three reminder stages worked out by you against policy 5.1, and the plan's date before the run's in your history
- [ ] `NOTES.md`: how you sorted the three jobs, the Description test, and how the apps compared
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] Committed, tagged `step-11-done` and pushed

## References

- [Chapter 0.3: AI Fluency](https://agentfactory.panaversity.org/how-ai-works/ai-fluency/overview/)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md), section 5

---

[← Step 10: Markdown: One Page, Checked](../step-10-markdown/) · [Roadmap](../README.md#roadmap) · [Step 12: Critical Thinking and Judgment →](../step-12-critical-thinking/)
