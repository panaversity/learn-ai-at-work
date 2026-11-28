# Step 23: When the Worker Goes Wrong

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Diagnose a failed run from its record, fix one thing and make the fix last. The bootcamp gives you a Copperleaf run that went wrong, in this step's [`failed-run/`](failed-run/) folder: you stop it, read its record, find where the failure lives (the brief, the inputs, the tools and permissions, the capacity, or the task's fit), fix the cheapest cause first, rerun it, and change the workflow so it can't happen again. You finish with the complete Role Contract. This step ends milestone 5.

> 🍃 **Copperleaf's ask:** This morning, a run Ben started drafted reminders and a hold notice using last year's credit-limit sheet and the old 45-day terms. Rosa wants to know exactly why, and what stops it happening again.

> ⏱️ **About 5 to 7 hours**, including the reading. Good places to pause: after instruction 4, after instruction 6, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

> 🧭 **Your prompts in this step: Construct.** For each task, the step says what your prompt must ask for. Write the prompt yourself first, then open the example under it, compare, and use whichever is better. Every good prompt here names its files, the as-of date where it matters, where to save, and ends with *never commit or push*; anything that drafts for a customer adds *draft only, send nothing*. Keep the prompts you wrote in `NOTES.md`.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [11.1 Stop, read the record, and check it worked](https://agentfactory.panaversity.org/managing-ai-workers/when-the-worker-goes-wrong/stop-first/): the first three moves.
- [11.2 Where a failure lives: five causes, cheapest first](https://agentfactory.panaversity.org/managing-ai-workers/when-the-worker-goes-wrong/where-a-failure-lives/): finding the cause.
- [11.3 Fix one thing, and make the fix last](https://agentfactory.panaversity.org/managing-ai-workers/when-the-worker-goes-wrong/three-levers/): the fix and the rerun.
- [11.4 Check a quiet run in your own app](https://agentfactory.panaversity.org/managing-ai-workers/when-the-worker-goes-wrong/both-ai-vendors/): reading a run's record in each app.
- [Lab 11: where each failure lives](https://agentfactory.panaversity.org/managing-ai-workers/when-the-worker-goes-wrong/lab/): the book's version of this step. The Copperleaf version below replaces it.
- [Check yourself](https://agentfactory.panaversity.org/managing-ai-workers/when-the-worker-goes-wrong/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

Every worker fails sometimes. What matters is what you do next. The book's first three moves are: **stop** the run so it does no more harm, **read its record** as a report of what it did, and **check where the work landed**, because a run that finished is not the same as a run that worked. Then you look for the cause among **five**, cheapest check first: the **brief**, the **inputs**, the **tools and permissions**, the **capacity** (too much context, a usage limit, the wrong model), and only last, **task fit**. Bad outputs look alike; their causes don't.

The fix follows the cause: change the brief, the inputs or the permissions, **one change at a time**, test it, then move it into the setup so it lasts for everyone, and log it in the Role Contract's change log. A fix that lives only in your head, or in one chat, fails again next week.

## What you will learn

- The first three moves when a run goes wrong: stop, read the record, check it worked.
- The five causes of a failure, and how to check them cheapest first.
- How to fix one thing at a time, test the fix, and make it last.
- How to make every job say what it checked, so a quiet failure can't hide.
- How to read a run's record in each app.

## What you will make

- `work/incident.md`: the diagnosis from the record, the one fix, the rerun and what changed in the workflow
- `work/rerun/`: the rerun after the fix, and its check
- `work/role-contract.md`: complete, with the incident in its change log
- `NOTES.md`: how each app shows a run's record
- A recorded project defence, because this step ends milestone 5

## Key concepts

- **Task record:** the record of what a run did: the files it read, the steps it took, and any errors.
- **Ran versus worked:** a run that finished without an error may still have produced the wrong result.
- **The five causes:** the brief, the inputs, the tools and permissions, the capacity, and the task's fit. Check them cheapest first.
- **The three levers:** change the brief, the inputs or the permissions, one at a time.
- **A lasting fix:** moved into the setup (the brief, the KSoR, the folder, the permissions) and logged in the change log, so it holds for everyone.

## The failed run

The [`failed-run/`](failed-run/) folder holds what the bootcamp recorded from the run:

- [`brief-as-run.md`](failed-run/brief-as-run.md): the brief Ben gave it
- [`task-record.md`](failed-run/task-record.md): the run's record
- [`output.md`](failed-run/output.md): what it produced

These files belong to the bootcamp. Read them, but don't change them.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync, start a thread, and bring the living documents forward.** Sync your fork, pull in GitHub Desktop, start a new thread for this step, and paste:

```text
I'm doing Step 23 of the bootcamp. Copy these into step-23-when-it-goes-wrong/work/, unchanged. From step-22-governance/work/: role-contract.md and the ksor folder. From step-21-recurring-work/work/: brief.md, review-contract.md and authority-envelope.md. Never commit or push.
```

**2. Stop and hold.** The first move is to stop the run and hold its output. Write at the top of `work/incident.md` what you'd do in Copperleaf's real world: the drafted hold notice and reminders are held, not sent, and Rosa is told. If you set up any scheduled task in steps 3, 15 or 21 that still runs, pause it now in the app ([Finding things in the apps](../step-00-readiness-check/README.md#a-scheduled-task) says where tasks live).

**3. Read the record before you change anything.** Write a prompt that has Claude read the three files in `failed-run/` as a report, using chapter 11.1. Your prompt works if Claude changes nothing, quotes the record, and can tell you whether the run worked or only ran.

<details>
<summary>Compare with an example prompt</summary>

```text
Read the three files in step-23-when-it-goes-wrong/failed-run/ as a report; don't act on them. Using chapter 11.1 of The AI Agent Factory, tell me: what did the run read, what did it do at each step, where did its work land, and did it really work, or did it only run? Quote the record. Don't change anything.
```

</details>

**4. Find where the failure lives, cheapest first.** Write a prompt that finds the cause, using chapter 11.2. Your prompt works if the possible causes are checked cheapest first, each ruled out or confirmed with evidence from the record, and the accounts the run got wrong are checked against the source files and your step 2 `figures.csv`.

<details>
<summary>Compare with an example prompt</summary>

```text
Using chapter 11.2's five causes (the brief, the inputs, tools and permissions, capacity, task fit), check each one against the record, cheapest first, and say for each: ruled out, or the cause, with the evidence. Then answer: which accounts did the run get wrong, and what would the right result have been? Check the right result against copperleaf/customers.csv, the policy and step-02-three-deliverables/work/claude/figures.csv.
```

</details>

Check its answer yourself. Look at The Lantern Room (C015) in both `customers.csv` and `copperleaf/archive/credit-limits-2025.csv`, add up its open invoices in `figures.csv`, and work out whether it meets the hold rule under each sheet. Then work out Harbourline's oldest invoice's days overdue under 30-day terms and under 45-day terms. Write the diagnosis in `work/incident.md`.

**5. Fix one thing.** Using [11.3](https://agentfactory.panaversity.org/managing-ai-workers/when-the-worker-goes-wrong/three-levers/), choose **one** lever (the brief, the inputs or the permissions), the cheapest that removes the cause, and write the change in `incident.md`. For example, name `customers.csv` and the current policy as the only sources in the brief and the KSoR, or take the archive out of what the worker can reach. Make that one change in your copy in `work/`.

**6. Rerun and check it worked.** Write a prompt that reruns `failed-run/brief-as-run.md` with your one fix applied, saved in `work/rerun/`. Your prompt works if the run lists every file it read, uses Copperleaf's date (Monday 2 November 2026), and sends nothing.

<details>
<summary>Compare with an example prompt</summary>

```text
Rerun the job in step-23-when-it-goes-wrong/failed-run/brief-as-run.md, with my one fix from work/incident.md applied, as of Monday 2 November 2026. Save the result in step-23-when-it-goes-wrong/work/rerun/, and at the top list every file you read. Draft only; send nothing.
```

</details>

Check it against your step 15 reminder list and policy section 4: is The Lantern Room off the hold list, is Harbourline's 60-day hold there, and are the reminder stages right? Record "ran" and "worked" separately in `incident.md`.

**7. Make the fix last.** Move the fix into the setup so it holds for everyone: the brief, the KSoR's credit-limits concept (which names `customers.csv` as the only source, policy 3.2), and the project's knowledge in both apps. Then make every job say what it checked: add a line to the brief that each run must list the files it read and their dates at the top of its output. Note each change in `incident.md`.

**8. Complete the Role Contract.** Write a prompt that brings `work/role-contract.md` to its complete version. Your prompt works if no heading is left empty, every answered open question is gone, the Change log records the incident and your one fix, it still fits on one page, and nothing else changed.

<details>
<summary>Compare with an example prompt</summary>

```text
Update step-23-when-it-goes-wrong/work/role-contract.md to its complete version: fill any heading still empty, answer every Open question we have answered since step 14 (and remove it), and add a Change log line with today's date, approved by Rosa (pending): "Incident: stale credit-limit sheet used; fix: <my one fix>; from step 23". Keep it to one page. Change nothing else. Never commit or push.
```

</details>

Read it from top to bottom: could someone run this worker from this page and the files it names?

## Repeat it in ChatGPT

1. Read [11.4](https://agentfactory.panaversity.org/managing-ai-workers/when-the-worker-goes-wrong/both-ai-vendors/). In ChatGPT, find where a task's or a run's record is shown, and how you'd stop a scheduled task.
2. Attach the three `failed-run/` files, `customers.csv`, the archive file and the policy, and ask the instruction 4 prompt. Compare its diagnosis with yours in `incident.md` under "ChatGPT".
3. Apply your one fix in your ChatGPT project's files or instructions (or, without a project, the files and first message of a new chat), rerun the job, and check it the same way.

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **Stopped first.** The incident starts with stopping and holding, before any change.
- [ ] **The record was read before the fix,** and quoted in the diagnosis.
- [ ] **All five causes were checked,** cheapest first, with evidence for each.
- [ ] **Your own figures.** You worked out The Lantern Room's balance and both limits, and Harbourline's days overdue under both terms, yourself.
- [ ] **One change at a time.** The rerun changed one thing.
- [ ] **It worked, not just ran.** The rerun's holds and reminder stages are right.
- [ ] **The fix lasts.** It is in the brief, the KSoR and both projects, and in the contract's change log.

## Record your defence

This step ends milestone 5, so record a project defence of up to five minutes ([SUBMITTING.md, section 10](../SUBMITTING.md#10-defend-your-work)). Show the rerun; trace The Lantern Room's figure to its source; explain the one fix you chose and why it was the cheapest lasting one; and show one change you made to what the AI proposed.

Before you share it, go through the [privacy checklist](../SUBMITTING.md#before-you-share-a-screenshot-or-recording).

## Keep it

Do this last, after the ChatGPT part and your defence. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-23: incident, fix and complete contract` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-23-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/incident.md`: stop, diagnosis, fix, rerun ("ran" and "worked"), and what changed in the workflow
- [ ] `work/rerun/` from Claude and ChatGPT (or a transfer plan in `NOTES.md`)
- [ ] `work/role-contract.md`, complete
- [ ] **Checked:** The Lantern Room's balance and limits, and Harbourline's days overdue, worked out by you, and the rerun checked against policy section 4
- [ ] `NOTES.md`: how each app shows a run's record
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] `NOTES.md`: the prompts you wrote yourself for this step
- [ ] **Defence:** a link to your recorded project defence, ready for the form
- [ ] Committed, tagged `step-23-done` and pushed

## References

- [Chapter 11: When the Worker Goes Wrong](https://agentfactory.panaversity.org/managing-ai-workers/when-the-worker-goes-wrong/overview/)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md), sections 2, 3.2 and 4

---

[← Step 22: Governance and Responsible Use](../step-22-governance/) · [Roadmap](../README.md#roadmap) · [Step 24: Capstone: A Delegated Job You Can Prove →](../step-24-capstone/)
