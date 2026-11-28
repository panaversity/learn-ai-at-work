# Step 21: Work That Runs Without You

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Decide which receivables work should run without you, and govern it. You set up two recurring jobs, a Monday aged-debt report on a schedule and a check that starts when a payment arrives that matches no invoice, each with its trigger, inputs, limits and the person who checks it. You also decide what the worker may do unasked, explain to the team what runs and who still checks, and carry one job from question to plan: a researched, checked plan for Amira on how Copperleaf could get paid faster.

> 🍃 **Copperleaf's ask:** Rosa does not want to remember to start the Monday report, but she also does not want work happening that nobody looks at.

> ⏱️ **About 7 to 9 hours**, including the reading. Good places to pause: after instruction 4, after instruction 6, after instruction 8, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

> 🧭 **Your prompts in this step: Construct.** For each task, the step says what your prompt must ask for. Write the prompt yourself first, then open the example under it, compare, and use whichever is better. Every good prompt here names its files, the as-of date where it matters, where to save, and ends with *never commit or push*; anything that drafts for a customer adds *draft only, send nothing*. Keep the prompts you wrote in `NOTES.md`.

> 🆓 **On the free route:** run each job by hand at its trigger (Monday 7:00, and when you create the inbox file), and mark both runs **simulated**. Everything else in the step works as written.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [9.1 Decide what runs without you, and who does each step](https://agentfactory.panaversity.org/managing-ai-workers/work-that-runs-without-you/fit-the-workflow/): whether it is an agent problem at all.
- [9.2 Give every run what it needs](https://agentfactory.panaversity.org/managing-ai-workers/work-that-runs-without-you/scheduled-and-event-triggered/): scheduled and triggered work.
- [9.3 Govern what it does unasked](https://agentfactory.panaversity.org/managing-ai-workers/work-that-runs-without-you/governing-initiative/): initiative you did not ask for.
- [9.4 Explain what runs, and who still checks](https://agentfactory.panaversity.org/managing-ai-workers/work-that-runs-without-you/explaining-value-and-limits/): the note you write for the team.
- [9.6 The worker in a shared room](https://agentfactory.panaversity.org/managing-ai-workers/work-that-runs-without-you/shared-room/): who a shared worker works for, and whose approval counts.
- [9.7 One deliverable, from question to plan](https://agentfactory.panaversity.org/managing-ai-workers/work-that-runs-without-you/one-deliverable/): a research and analysis job carried through to a plan someone can act on.
- [9.5 Set up the recurring run in your own app](https://agentfactory.panaversity.org/managing-ai-workers/work-that-runs-without-you/both-ai-vendors/): setting up both jobs.
- [Lab 9: when nobody is watching](https://agentfactory.panaversity.org/managing-ai-workers/work-that-runs-without-you/lab/): the book's version of this step. The Copperleaf version below replaces it.
- [Check yourself](https://agentfactory.panaversity.org/managing-ai-workers/work-that-runs-without-you/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

A **standing** worker starts its own work, on a schedule or when something happens. That is exactly what Rosa wants, and exactly what she fears: work nobody started is easy to stop checking. The book's answer has four parts. First, decide what should run at all, and **who does each step**: the worker, or a person. Second, give every run what it needs, because each run starts fresh: the brief, the approved knowledge, and a **case file** that tells it what earlier runs found. Third, govern **initiative**: what the worker may do when nobody asked, on the same four rungs as the Authority Envelope. Fourth, tell the people who rely on it what runs, what it never does, and who still checks, by name.

A recurring job that fails quietly is worse than no job, because people stop looking. So every run reports what it checked, and a person notices when a report doesn't arrive.

## What you will learn

- Three gates before any recurring work, and a delegation map of who does each step.
- How scheduled and event-triggered runs differ, and five facts every unwatched run must be designed for.
- The case file each run reads first, and why the record is not the truth now.
- The initiative ladder, and an execute rule for each kind of act.
- The six things to tell the people who rely on the work.
- How to carry one deliverable through four stages, with two checks at each.

## What you will make

- `work/delegation-map.md`: the weekly receivables workflow, step by step, with who does each step and why
- `work/jobs/monday-report.md` and `work/jobs/unmatched-payment-check.md`: each job's trigger, inputs, case file, limits, the person who checks it, and how a failure shows
- `work/runs/`: one run of each job, and its review
- `work/initiative.md`: what the worker may do unasked, rung by rung, with the execute rule
- `work/note-for-the-team.md`: one page on what runs and who still checks
- `work/get-paid-faster-plan.md`: one deliverable from question to plan, with its sources cited and its figures worked out from Copperleaf's files, as in the book's [Lab 9, Task 13](https://agentfactory.panaversity.org/managing-ai-workers/work-that-runs-without-you/lab/#task-13-one-plan-for-dave)
- `work/role-contract.md`: version 8, with both jobs under Triggers
- `NOTES.md`: how the apps compared

## Key concepts

- **Delegation map:** each step of a workflow, with who does it (the worker or a named person) and what supports it.
- **Scheduled and event-triggered:** a run started by the clock, or by something happening, such as a payment arriving.
- **Case file:** the record each run reads first, so it knows what earlier runs found; it shows the latest known, with its date, not the truth now.
- **Initiative ladder:** observe, recommend, draft and execute, for work nobody asked for; initiative stays inside the authority already granted.
- **Execute rule:** for each kind of act, one of: do it without asking, do it if pre-approved, ask first, or hand it to a person.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync, start a thread, and bring the living documents forward.** Sync your fork, pull in GitHub Desktop, start a new thread for this step, and paste:

```text
I'm doing Step 21 of the bootcamp. Copy step-20-knowledge-and-state/work/role-contract.md, brief.md, review-contract.md, authority-envelope.md and the ksor folder to step-21-recurring-work/work/, unchanged. Never commit or push.
```

**2. Who does each step.** Write a prompt for a delegation map of Copperleaf's weekly receivables work, saved as `work/delegation-map.md`, using chapter 9.1. Your prompt works if the map covers every step from the payments arriving to the reminders going out, gives each step a doer by name and its policy section, passes 9.1's gates and avoids its common mapping errors, and leaves with people everything the policy reserves for them.

<details>
<summary>Compare with an example prompt</summary>

```text
Using chapter 9.1 of The AI Agent Factory, make step-21-recurring-work/work/delegation-map.md for Copperleaf's weekly receivables work, from the payments arriving to reminders going out. For each step: who does it (the worker or a named person: Rosa, Ben or me), the three gates (may it go to a worker; who should own it; what supports it), and the policy section that applies. Show the three common mapping errors from 9.1, if any appear. Keep sending, approving holds, refunds and anything about bank details with people. Never commit or push.
```

</details>

Check each "person" step against policy section 11. Then add a **baseline**: how long the weekly work takes by hand today (make a reasonable estimate and label it an estimate), so you can tell later if the new way is better.

**3. Design the two jobs.** Write a prompt for two job sheets in `work/jobs/`, `monday-report.md` (scheduled every Monday at 7:00) and `unmatched-payment-check.md` (started when a payments file arrives in `work/inbox/`), and for `work/case-file.md`, what is known today. Your prompt works if Ben could run either job from its sheet without asking you: what starts it, what it reads first, what it may do, what it writes back, and who checks it by when. The payment check must never allocate a payment itself (policy 8), and the case file must hold everything still open from earlier steps.

<details>
<summary>Compare with an example prompt</summary>

```text
Write two job sheets in step-21-recurring-work/work/jobs/, following chapter 9.2:
1. monday-report.md: scheduled every Monday at 7:00. It produces the aged-debt report (as in step 7) and a list of what needs a person.
2. unmatched-payment-check.md: event-triggered, starting when a new payments file arrives in step-21-recurring-work/work/inbox/. For each payment, it checks the case file and the open invoices, and either proposes a match with the evidence, or lists it as unallocated for Ben (policy 8.1, 8.2). It never allocates a payment itself.
For each job: the trigger, the inputs (the brief, the KSoR concepts, and the case file it reads first: work/case-file.md), what it may do (from the Authority Envelope), what it writes back to the case file, who checks the result and by when, and how a failure shows (it must never fail silently). Also create work/case-file.md with what we know today: last week's unallocated payments, Riverside's confirmed payment from step 7, and the disputed INV-4199. Never commit or push.
```

</details>

**4. Write each job's checks first.** Add a short review contract to the end of each job sheet (what is checked, evidence, success, what stops it), and commit the two job sheets and the case file on their own (`step-21: job sheets and checks, before the runs`).

**5. Set up and run the Monday report.** Set it up as a scheduled task ([Finding things in the apps](../step-00-readiness-check/README.md#a-scheduled-task) shows where), following [9.5](https://agentfactory.panaversity.org/managing-ai-workers/work-that-runs-without-you/both-ai-vendors/), with an instruction that points to `work/jobs/monday-report.md`. Run it once (use **Run now** if the app offers it, or wait for the time). Save the result in `work/runs/monday-report/`, and review it against its checks.

**6. Trigger the payment check.** Create `work/inbox/payments-2026-11-03.csv` with this content (a payment that arrived on Tuesday), using any text editor or by asking Claude:

```text
payment_id,date_received,payer_name,amount,reference,method
PAY-9043,2026-11-03,Harbour Line Hotels,1414.76,HARBOURLINE OCT,Bank transfer
```

If your app can start a job when a file arrives, let it. If not, run the job by hand, and say so in `NOTES.md`: the book notes that not every app has every trigger. Save the result in `work/runs/payment-check/`. The payer's name doesn't match the customer list exactly and the reference isn't an invoice number: what should it do? Review it against its checks.

**7. Govern initiative.** Write a prompt for `work/initiative.md`: what the worker may do about things it notices unasked while running these jobs. Your prompt works if each case it lists has a rung and a rule for what happens next, and nothing goes above the Authority Envelope.

<details>
<summary>Compare with an example prompt</summary>

```text
Using chapter 9.3, write step-21-recurring-work/work/initiative.md: things the worker might notice while running these jobs without being asked (for example, an account that now meets the hold rule, a customer whose email address changed, an old file in the folder), and for each, the highest rung it may reach unasked, and the execute rule (do it, do it if pre-approved, ask first, or hand it to a person). Initiative may never go beyond the Authority Envelope.
```

</details>

**8. Explain it to the team.** Write a prompt for `work/note-for-the-team.md`, one page for Rosa and Ben, using chapters 9.4 and 9.6. Your prompt works if Ben could run the week from the note alone, it covers everything 9.4 asks a note like this to cover, and it avoids the words 9.4 warns against.

<details>
<summary>Compare with an example prompt</summary>

```text
Using chapter 9.4, write step-21-recurring-work/work/note-for-the-team.md, one page for Rosa and Ben covering the six things: what runs and when, what it reads, what it never does, what a person still checks (by name and by when), how we will know it failed, and what it is worth, measured (only claims we can back). Avoid the words 9.4 says to avoid. Add who may ask the worker for what (9.6).
```

</details>

**9. One deliverable, from question to plan.** Amira asks: "How could Copperleaf get paid faster?" Carry it through the four stages of [9.7](https://agentfactory.panaversity.org/managing-ai-workers/work-that-runs-without-you/one-deliverable/), with two checks at each stage, in `work/get-paid-faster-plan.md`. The figures (how much is overdue, which customers, how late) must be worked out from Copperleaf's files, and every outside claim (common practice, for example) cited with a source you opened. End with a plan Amira can act on: three actions, who owns each, and how you will know each worked.

**10. Draft 8 of the contract.** Write a prompt that adds both jobs to `work/role-contract.md` as Draft 8. Your prompt works if only the parts the jobs touch change, and the Change log records the draft, the date and who must approve it.

<details>
<summary>Compare with an example prompt</summary>

```text
In step-21-recurring-work/work/role-contract.md, add both jobs under Triggers and Responsibilities, set Kind to "Standing", and add a Change log line with today's date, approved by Rosa (pending): "Draft 8: two recurring jobs, from step 21". Change nothing else.
```

</details>

## Repeat it in ChatGPT

1. Set up the Monday report as a scheduled task in ChatGPT (if your plan has scheduled tasks), with the job sheet and the files it needs attached to the project. Run it once and review it in `work/runs/chatgpt/`.
2. Run the payment check in ChatGPT by hand with the inbox file, and review it.
3. In `NOTES.md`, compare the two apps' controls for recurring work: schedules, triggers, where results land, and how you would notice a failure.

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **Every person-only step stays with a person** in the delegation map, checked by you against policy section 11.
- [ ] **The checks came first.** The job sheets and their checks are committed before the runs.
- [ ] **The Monday report is right.** Its totals match your checked step 2 figures.
- [ ] **The payment check didn't allocate.** PAY-9043 is proposed with its evidence, or held as unallocated, and listed for Ben; nothing was applied.
- [ ] **Initiative stays inside the envelope.** No rung in `initiative.md` is higher than the Authority Envelope allows.
- [ ] **The plan's figures are yours.** You worked out each figure in the plan from Copperleaf's files, and opened every cited source.

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-21: recurring work` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-21-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/delegation-map.md`, with a baseline
- [ ] `work/jobs/` with both job sheets and their checks, committed before the runs, and `work/case-file.md`
- [ ] `work/runs/` with one run of each job and its review, from Claude and ChatGPT (or a transfer plan in `NOTES.md`)
- [ ] `work/initiative.md` and `work/note-for-the-team.md`
- [ ] `work/get-paid-faster-plan.md`
- [ ] `work/role-contract.md` (Draft 8)
- [ ] **Checked:** the Monday report's totals compared with your step 2 figures, and every figure in the plan worked out by you
- [ ] `NOTES.md`: how the apps compared
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] `NOTES.md`: the prompts you wrote yourself for this step
- [ ] Committed, tagged `step-21-done` and pushed

## References

- [Chapter 9: Work That Runs Without You](https://agentfactory.panaversity.org/managing-ai-workers/work-that-runs-without-you/overview/)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md), sections 8 and 11

---

[← Step 20: Context, Memory, Knowledge and State](../step-20-knowledge-and-state/) · [Roadmap](../README.md#roadmap) · [Step 22: Governance and Responsible Use →](../step-22-governance/)
