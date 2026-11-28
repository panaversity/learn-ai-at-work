# Step 24: Capstone: A Delegated Job You Can Prove

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Bring everything together on one real job, the way the book's Part II capstone does. For Copperleaf's receivables work (or a task from your own role, rebuilt with made-up data), you write the Four-Part Brief, answer from your own KSoR, keep the worker inside its Authority Envelope, and write the review contract before you delegate. You run the job in Claude, repeat it in ChatGPT, review the result against the contract and trace every claim. Then you sit the book's PCAO-F sample exam. This is your evidence for the book's portfolio milestone A, Manager.

> 🍃 **Copperleaf's ask:** Copperleaf is ready to let the Receivables Worker take the weekly run for real. Before Amira signs off, she wants one complete job she can audit from brief to result.

> ⏱️ **About 12 to 16 hours**, including the reading. Good places to pause: after instruction 3, after instruction 5, after instruction 7, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later. Sit the sample exam (instruction 8) in one sitting, against the clock, and record the defence in one take.

> 🆓 **On the free route:** run the job in a fresh chat with the brief, the envelope, the five concepts and the files the brief names attached, and say so in `audit-pack.md`. With one app, write the transfer plan the ChatGPT part describes. The README's [evidence table](../README.md#what-counts-as-evidence-on-each-route) shows what each counts as.

> 🧭 **Your prompts in this step: On your own.** Apart from copying your files forward, there are no prompts to copy. Each instruction gives the task and its checks; you write the prompt, run it and verify the result. Keep the prompts you wrote in `work/prompts.md`, because your defence shows one of them.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [Part II: the part capstone](https://agentfactory.panaversity.org/managing-ai-workers/overview/#the-part-capstone): what the capstone is and how it is graded.
- [Appendix C. Preparing for PCAO-F and CCAO-F](https://agentfactory.panaversity.org/appendices/exams/associate-foundations/overview/): the 21 skills and where the book teaches each.
- [PCAO-F sample exam](https://agentfactory.panaversity.org/appendices/exams/associate-foundations/sample-exam/): 70 questions against the clock, with a score for each domain.
- [Certification and Portfolio Roadmaps](https://agentfactory.panaversity.org/certification-and-portfolio-roadmaps/): where PCAO-F and milestone A lead next.
- [From Skills to Income](https://agentfactory.panaversity.org/from-skills-to-income/overview/): how this work becomes income.

## Why this step matters

Everything so far has been practice for one moment: handing a real job to an AI Worker and being able to prove, to someone who wasn't there, that it was briefed, bounded, checked and signed. The book's capstone is graded on six criteria, each Not yet (1), Meets (2) or Exceeds (3): **outcome**, **evidence**, **governance**, **portability**, **communication**, and Part II's own, **the review contract was written before delegation**. To pass you need at least Meets on every criterion and 14 of 18 points. A contract written after the run fails, however good the result. A good answer reached by an action the Authority Envelope didn't allow fails governance.

Amira's request is the same test in plain words: one complete job she can audit from brief to result. When you can do that, you are ready for PCAO-F, and you have the first piece of a portfolio an employer or client can see.

## What you will learn

- How to put the brief, the KSoR, the envelope and the review contract together on one job.
- How to prove the order of your work with your commit history.
- How to present delegated work so someone else can audit it.
- Where you stand on every PCAO-F domain.

## What you will make

All in this step's `work/` folder:

- `brief.md`: the Four-Part Brief for the job
- `ksor/`: the five approved concepts the worker answers from
- `authority-envelope.md`: what the worker may do on this job
- `review-contract.md`: committed **before** the run
- `runs/claude/` and `runs/chatgpt/`: both runs, with their records
- `review.md`: the review against the contract, every claim traced, with verdicts
- `audit-pack.md`: one page for Amira that walks from the brief to the signed result, linking every file
- `self-assessment.md`: your own score on the six criteria, with evidence for each
- `NOTES.md`: your PCAO-F sample exam scores by domain, and what you will revise
- A recorded project defence of up to ten minutes

## Key concepts

- **Part capstone:** one piece of work that uses everything in Part II, graded on the book's six-criterion rubric.
- **Portfolio milestone A, Manager:** the book's first portfolio milestone; the capstone, its review contract and your KSoR are the evidence.
- **Audit pack:** the files and a one-page guide that let someone who wasn't there check the job from brief to result.
- **Portability:** the job would run the same on the other vendor's app from the same files.
- **Order of work:** brief, knowledge, envelope and review contract first, then the run; your commit history proves it.

## Choose your job

Do one of these, and say which in `NOTES.md`:

- **Copperleaf (default):** the weekly receivables run for Monday 2 November 2026, from matching last week's payments to drafting the reminders and any hold proposal, ready for Rosa to sign.
- **Your own role:** a recurring task from your own work, rebuilt with made-up (synthetic) data, with five approved concepts from your field. Write the data from scratch: real records with the names changed aren't safe, because amounts, dates and other details can still identify people and companies ([10.2](https://agentfactory.panaversity.org/managing-ai-workers/governance-and-responsible-use/can-this-data-go-in/)), and your fork is public. If you aren't sure, use Copperleaf.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="../assets/delegated-job-dark.png">
  <img src="../assets/delegated-job-light.png" alt="Before the run, write and commit four things: the brief, the knowledge (KSoR concepts), the Authority Envelope and the review contract. Then the worker runs the job. You read its record first, then run four checks in order: recompute, trace, match and compare. Each output gets a verdict: ready to use, requires revision, or requires human correction. A person signs before anything leaves the company. You learn the four documents one at a time in steps 17 to 20, in a different order; on a real job, all four are ready before the run." width="100%">
</picture>

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync, start a thread, and bring the living documents forward.** Sync your fork, pull in GitHub Desktop, start a new thread for this step, and paste:

```text
I'm doing Step 24, the capstone. Copy step-23-when-it-goes-wrong/work/role-contract.md, brief.md, review-contract.md, authority-envelope.md and the ksor folder to step-24-capstone/work/, unchanged. Don't change step 23. Never commit or push.
```

Using your own role? Paste this instead:

```text
I'm doing Step 24, the capstone, on a task from my own role. Help me create step-24-capstone/work/ with a brief, five KSoR concepts, an Authority Envelope and a review contract for it, one at a time, using chapters 5 to 8 of The AI Agent Factory. Ask me about the task first, then help me make up realistic synthetic data for it; never ask me for real data. Never commit or push.
```

**2. Tighten each document for this one job.** Write a prompt that has Claude read the brief, the KSoR concepts, the Authority Envelope and the Role Contract in `work/`, and list, without fixing anything, whatever is missing, out of date or inconsistent between them for the weekly run of Monday 2 November 2026 (for example, a rung the brief contradicts, or a concept still in draft).

Fix each point yourself or by asking Claude for that one change. Every concept the worker uses must be stable and approved.

**3. Write the review contract, and commit it first.** Update `work/review-contract.md` for this job: what must be checked, what evidence comes back, what counts as success, and what stops the worker. Then, in GitHub Desktop, commit **the brief, the KSoR, the envelope and the review contract on their own**, with the summary `step-24: brief, KSoR, envelope and review contract, before the run`, and push. This commit is the proof the capstone's sixth criterion asks for.

**4. Run it in Claude.** In your `Copperleaf Receivables Worker` project from step 20 (refreshed with this step's concepts), or in a fresh thread of your bootcamp project, write the run prompt yourself. It must: point to `work/brief.md` as the job and say the as-of date; keep the worker inside `work/authority-envelope.md`; allow rule answers only from `work/ksor/`; stop where the brief says; save the results in `work/runs/claude/` with a `record.md` listing every file read (with its date) and every step; and say draft only, send nothing.

Approve each stop only after checking that stage.

**5. Review against the contract.** In `work/review.md`, read the record first, then run the four checks in order (recompute, trace, match, compare), trace every claim to its file or concept, and give each output a verdict. Recompute the totals yourself from the source files.

**6. Write the audit pack.** Write `work/audit-pack.md`, one page for Amira, yourself or with a prompt you write. It must give the job in one sentence; then, in order, the brief, the knowledge, the envelope, the review contract (with the commit that shows it came first), the runs, the review and its verdicts, and who signs what; link each file; and say plainly what a person checked and what nobody did.

Read it as Amira would. Could she audit the job from this page alone?

**7. Score yourself.** In `work/self-assessment.md`, score each of the six criteria (1, 2 or 3) with the evidence: a file, a line or a commit. Be honest: a 1 you find now is one you can fix before you submit.

**8. Sit the sample exam.** Take the [PCAO-F sample exam](https://agentfactory.panaversity.org/appendices/exams/associate-foundations/sample-exam/) on your own, without AI help, against the clock. Record your score for each domain in `NOTES.md`, save a screenshot of the results page in `work/` as evidence, and for any domain under 70 percent, the book sections you will revise ([Appendix C](https://agentfactory.panaversity.org/appendices/exams/associate-foundations/overview/) maps each skill to its chapter).

## Repeat it in ChatGPT

1. In your ChatGPT `Copperleaf Receivables Worker` project (step 20), or a new chat if you have no project, refresh the five concepts and attach the brief, the envelope and the files the brief names.
2. Run the same job with your run prompt from instruction 4, stopping where the brief says, and save the results in `work/runs/chatgpt/`.
3. Review it against the same contract in a "ChatGPT" section of `review.md`.
4. In `audit-pack.md`, add one paragraph on portability: did the same files give the same result on both vendors? Where they differed, why?

With only one app, write a transfer plan in `NOTES.md` instead: the inputs, instructions, permissions and checks the other app would need, marked *planned, not tested*. Portability is a graded criterion, so make it complete. The capstone uses only its 18-point rubric ([SUBMITTING.md, section 9](../SUBMITTING.md#9-how-each-step-is-graded)): for portability, a complete transfer plan can reach Meets, but Exceeds needs a real run in both apps.

## Check it

- [ ] **The order is proven.** In **History**, the brief, KSoR, envelope and review contract are committed before anything in `work/runs/`.
- [ ] **Every concept used is stable and approved.**
- [ ] **The worker stayed in its envelope.** The record shows no action above its rung.
- [ ] **Recomputed by you,** to the cent, from the source files.
- [ ] **Every claim traced** to a file or a concept.
- [ ] **Both runs reviewed** against the same contract, or, with one app, a complete transfer plan marked *planned, not tested*.
- [ ] **Auditable from one page.** `audit-pack.md` links every file and says who signs.
- [ ] **Real data stays out.** If you used your own task, all its data is made up from scratch, not real data with the names changed.

## Record your defence

This is the final defence, up to ten minutes ([SUBMITTING.md, section 10](../SUBMITTING.md#10-defend-your-work)). Walk through the audit pack; show the commit that proves the review contract came first; trace one figure and one policy claim end to end; explain one governance decision; show one change you made to what the AI produced; and show one prompt you wrote yourself. Before you share it, go through the [privacy checklist](../SUBMITTING.md#before-you-share-a-screenshot-or-recording).

**Then the changed-data check (compulsory).** After you submit, your graders send you a changed copy of Copperleaf's files that you have never seen. Within 48 hours, rerun your job on it with the same brief, envelope and review contract, and check the result, either live with a grader watching or in one continuous, uncut recording ([SUBMITTING.md, section 9](../SUBMITTING.md#9-how-each-step-is-graded)). You don't graduate without it.

## Keep it

Do this last, after the ChatGPT run and your defence. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-24: capstone runs, review and audit pack` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-24-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/brief.md`, `work/ksor/`, `work/authority-envelope.md` and `work/review-contract.md`, committed before the run
- [ ] `work/runs/claude/` and `work/runs/chatgpt/` (or a complete transfer plan in `NOTES.md`)
- [ ] `work/review.md`, `work/audit-pack.md` and `work/self-assessment.md`
- [ ] **Checked:** totals recomputed by you from the source files, every claim traced, and the worker's actions checked against its envelope
- [ ] `NOTES.md`: which job you chose, and your PCAO-F sample exam scores by domain
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] `work/prompts.md`: every prompt you wrote for this step
- [ ] **Defence:** a link to your recorded project defence, ready for the form
- [ ] **Changed-data check:** done within 48 hours of receiving the files, supervised or in one continuous recording (you can't graduate without it)
- [ ] **Required reading:** you read [Sell the work, not the software](https://agentfactory.panaversity.org/from-skills-to-income/sell-the-work-not-the-software/) and the three pages after it, and `NOTES.md` says in a short paragraph which service you would sell first, to whom, and at what price per result
- [ ] Committed, tagged `step-24-done` and pushed

## References

- [Part II: Managing AI Workers](https://agentfactory.panaversity.org/managing-ai-workers/overview/)
- [Appendix C. Preparing for PCAO-F and CCAO-F](https://agentfactory.panaversity.org/appendices/exams/associate-foundations/overview/)
- [Certification and Portfolio Roadmaps](https://agentfactory.panaversity.org/certification-and-portfolio-roadmaps/) and [From Skills to Income](https://agentfactory.panaversity.org/from-skills-to-income/overview/)

---

[← Step 23: When the Worker Goes Wrong](../step-23-when-it-goes-wrong/) · [Roadmap](../README.md#roadmap)
