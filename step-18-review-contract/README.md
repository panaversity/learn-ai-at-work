# Step 18: The Review Contract

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Write the checks before you delegate, then hold the result to them. You agree a review contract for the weekly receivables run before it starts, run it, and apply the four checks: you recompute the numbers a decision depends on, trace every claim to its source, match every item, and compare the same fact everywhere it appears. Anything that cites nothing is treated as a warning. Last, you ask each app's research feature what the law and common practice say about charging interest on late payments, and check every citation it gives before Rosa may rely on it.

> 🍃 **Copperleaf's ask:** Last month a reminder went to a customer who had already paid. Rosa wants written checks that would have caught it, agreed before the next run, not after.

> ⏱️ **About 6 to 8 hours**, including the reading. Good places to pause: after instruction 3, after instruction 7, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

> 🧭 **Your prompts in this step: Modify.** The prompts are given, but they are a starting point. Before you paste each one, read it and change what doesn't fit what you found in earlier steps (a file name, a check, a limit). In `NOTES.md`, record one prompt you changed, and why.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [6.1 Agree the checks before you delegate](https://agentfactory.panaversity.org/managing-ai-workers/the-review-contract/agree-the-checks/): writing the contract first.
- [6.2 Run the four checks](https://agentfactory.panaversity.org/managing-ai-workers/the-review-contract/good-and-plausible/): good output versus output that only looks good.
- [6.3 Readers and the record](https://agentfactory.panaversity.org/managing-ai-workers/the-review-contract/work-you-did-not-watch/): checking work you did not watch.
- [6.4 Review the result in your own app](https://agentfactory.panaversity.org/managing-ai-workers/the-review-contract/both-ai-vendors/): using each app's tools to check.
- [Lab 6: the checks come first](https://agentfactory.panaversity.org/managing-ai-workers/the-review-contract/lab/): the book's version of this step. The Copperleaf version below replaces it.
- [Check yourself](https://agentfactory.panaversity.org/managing-ai-workers/the-review-contract/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

A result that reads well can still be wrong. If you decide what "good" means **after** you have seen the result, you tend to accept whatever it shows you. A **review contract** fixes that: four questions answered before the work starts (what must be checked, what evidence comes back, what counts as success, and what stops the worker). It is the last decision of the first 10 percent.

Then the review itself runs as four checks, in order: **recompute** the number someone acts on, from the source files; **trace** every claim to its source (a claim that cites nothing is a warning); **match** every item, so nothing is missing or doubled; and **compare** the same fact everywhere it appears. The checks end in one of three verdicts: *ready to use*, *requires revision* or *requires human correction*. From this step on, every review contract in this bootcamp is committed before its run.

## What you will learn

- The four questions of a review contract, and why it is written first.
- How deep a review should go, given what's at stake.
- The four checks, in order: recompute, trace, match and compare.
- The three verdicts, and what happens after each.
- How to read the record of work you didn't watch, and how to check a research report's citations.

## What you will make

- `work/review-contract.md`, committed **before** the run, so its date in your history comes first
- `work/run/`: the weekly run's results and its record
- `work/review.md`: the four checks, each finding, and the verdict
- `work/research-check.md`: the research report, each citation marked confirmed, wrong or not found, as in the book's [Lab 6, Task 12](https://agentfactory.panaversity.org/managing-ai-workers/the-review-contract/lab/#task-12-the-terms-report)
- `work/role-contract.md`: version 5, with the review contract under Evaluations
- `NOTES.md`: what each check caught, and how the apps compared

## Key concepts

- **Review contract:** the acceptance criteria set before delegation: what must be checked, what evidence comes back, what counts as success, and what stops the worker.
- **Recompute:** work out the number someone acts on again, from the source files.
- **Trace:** follow every claim to its source; a claim that cites nothing is a warning.
- **Match and compare:** every item appears once (match), and the same fact is the same everywhere it appears (compare).
- **Verdict:** ready to use; requires revision (the worker can fix it with a named change); or requires human correction (only a person has the fact, judgment or authority).

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="../assets/delegated-job-dark.png">
  <img src="../assets/delegated-job-light.png" alt="Before the run, write and commit four things: the brief, the knowledge (KSoR concepts), the Authority Envelope and the review contract. Then the worker runs the job. You read its record first, then run four checks in order: recompute, trace, match and compare. Each output gets a verdict: ready to use, requires revision, or requires human correction. A person signs before anything leaves the company. You learn the four documents one at a time in steps 17 to 20, in a different order; on a real job, all four are ready before the run." width="100%">
</picture>

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync, start a thread, and bring the living documents forward.** Sync your fork, pull in GitHub Desktop, start a new thread for this step, and paste:

```text
I'm doing Step 18 of the bootcamp. Copy step-17-four-part-brief/work/role-contract.md and step-17-four-part-brief/work/brief.md to step-18-review-contract/work/, unchanged. Never commit or push.
```

**2. Write the review contract, before anything runs.** Paste:

```text
Help me write step-18-review-contract/work/review-contract.md for the weekly receivables run in work/brief.md, following chapter 6.1 of The AI Agent Factory. It is a table with four rows, and I'll answer each:
1. What must be checked: the facts, figures and decisions that make the run usable, including the policy rules it applies.
2. What evidence comes back: what the run returns so I can check it without redoing it (a reason and a policy section on every row, a record of the files read).
3. What counts as success: tests the output must pass. Include: every payment appears exactly once; the totals match totals I work out from the source files, to the cent; no reminder for any invoice that is paid, credited or disputed; every claim traces to a source.
4. What stops the worker: cases where it must stop and ask.
Then add "How deep to review", using the stakes. Don't run anything. Never commit or push.
```

Answer each row in your own words. Rosa's ask (the reminder to a customer who had paid) must be caught by a success test.

**3. Commit it before the run.** In GitHub Desktop, commit `review-contract.md` on its own with the summary `step-18: review contract, before the run`, and push. This order is graded: a contract written after its run fails.

**4. Run the job.** In a fresh thread, paste:

```text
Run step-18-review-contract/work/brief.md, all stages, as of Monday 2 November 2026, stopping where it says. Save the results in step-18-review-contract/work/run/, with a record.md of every file you read and every step.
```

Approve the stop when stage 1 looks right.

**5. Read the record first.** Before the results, open `work/run/record.md`. What did it read? Did it touch any file the brief says not to use? Note it in `work/review.md`.

**6. Run the four checks, in order.** Write each finding in `work/review.md`:

- **Recompute:** work out the total of the payments, the total still open, and the overdue total yourself from the source files. Compare to the cent.
- **Trace:** pick every policy claim and five figures, and open each source. Mark anything that cites nothing.
- **Match:** every payment once; every overdue invoice either has a reminder or a reason it hasn't; no reminder for a paid or disputed invoice.
- **Compare:** the same figure in the summary, the files and the reminders is the same everywhere.

**7. Give a verdict.** At the end of `review.md`, give each output a verdict (ready to use, requires revision, or requires human correction) and say what happens next. For "requires revision", name the change to the brief or inputs; for "requires human correction", name the person.

**8. Check a research report.** Using Claude's research feature (or web search), paste:

```text
Research, for a small wholesale distributor that sells to businesses: what does the law in my country say about charging interest or fees on late payments between businesses, and what is common practice? Cite every source with a link.
```

Save the report, then make `work/research-check.md`: a table of every citation, with the claim it supports, and a column you fill in yourself after opening each link: *confirmed*, *wrong* (the page doesn't say that) or *not found*. Count how many were confirmed. Rosa may rely only on confirmed claims.

**9. Draft 5 of the contract.** Paste:

```text
In step-18-review-contract/work/role-contract.md, add the review contract (work/review-contract.md) under Evaluations, and a Change log line with today's date, approved by Rosa (pending): "Draft 5: review contract, from step 18". Change nothing else.
```

## Repeat it in ChatGPT

1. In your ChatGPT project (or, without one, a new chat with the same files attached), attach `brief.md`, the files it names and `review-contract.md`, and run the brief. Download its results into `work/run/chatgpt/`.
2. Run the same four checks on ChatGPT's results, in a "ChatGPT" section of `review.md`, with verdicts.
3. Run the research prompt in ChatGPT's research feature too, and check its citations in a second table in `research-check.md`.
4. In `NOTES.md`, compare: which app's run passed more checks, and which app's research had more confirmed citations?

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

> 🌍 **Optional: in your own field.** Before you hand Claude a task from your own field, write its review contract first: what will be checked, what evidence comes back, what counts as success and what stops it. Then run it on made-up material and review it against your own contract. See the README's [examples by profession](../README.md#your-client-copperleaf-supply).

## Check it

- [ ] **The contract came first.** In **History**, `review-contract.md` is committed before anything in `work/run/`.
- [ ] **Rosa's case is a test.** A success test would catch a reminder to a customer who has paid.
- [ ] **All four checks, in order,** with findings for each.
- [ ] **Recomputed by you,** to the cent, from the source files.
- [ ] **Every citation opened.** No research claim is marked confirmed unless you opened the page.
- [ ] **A verdict for every output,** with what happens next.

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-18: run, review and research check` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-18-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/review-contract.md`, committed before the run
- [ ] `work/run/` with results and record, from Claude and ChatGPT (or a transfer plan in `NOTES.md`)
- [ ] `work/review.md` with the four checks and verdicts
- [ ] `work/research-check.md` with every citation checked
- [ ] `work/role-contract.md` (Draft 5)
- [ ] **Checked:** the totals recomputed by you from the source files, and every research citation opened
- [ ] `NOTES.md`: what each check caught, and how the apps compared
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] `NOTES.md`: one prompt you changed before pasting it, and why
- [ ] Committed, tagged `step-18-done` and pushed

## References

- [Chapter 6: The Review Contract](https://agentfactory.panaversity.org/managing-ai-workers/the-review-contract/overview/)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md), sections 5.2 and 6.2

---

[← Step 17: The Four-Part Brief](../step-17-four-part-brief/) · [Roadmap](../README.md#roadmap) · [Step 19: The Authority Envelope →](../step-19-authority-envelope/)
