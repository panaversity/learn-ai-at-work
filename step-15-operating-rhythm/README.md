# Step 15: The 10-80-10 Operating Rhythm

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Run one piece of Copperleaf's work through the rhythm every delegated job follows: you set the intent, scope, authority and checks (the first 10 percent), the worker plans and executes (the middle 80), and you review the evidence, correct and approve (the final 10). You do it for the weekly reminder run, find which of the three common failures each weak run shows, and add the review checks to the Role Contract.

> 🍃 **Copperleaf's ask:** Rosa noticed that the same one-line request gives a good result one week and a bad one the next. She wants a routine that makes the good result normal.

> ⏱️ **About 5 to 6 hours**, including the reading. Good places to pause: after instruction 2, after instruction 4, after instruction 6, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

> 🧭 **Your prompts in this step: Modify.** The prompts are given, but they are a starting point. Before you paste each one, read it and change what doesn't fit what you found in earlier steps (a file name, a check, a limit). In `NOTES.md`, record one prompt you changed, and why.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [3.1 One rhythm in three parts](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/one-rhythm/): the rhythm itself.
- [3.2 The first 10 percent](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/first-10-percent/): intent, scope, authority and the review contract.
- [3.3 The middle 80 percent](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/middle-80-percent/): what the worker does while you are not watching.
- [3.4 The final 10 percent](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/final-10-percent/): evidence review, correction and approval.
- [3.5 Three scales: a task, a worker, a company](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/three-scales/): the same rhythm for one job and for a whole team.
- [3.6 The three failures](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/three-failures/): naming what went wrong in a weak run.
- [3.7 Schedule the rhythm in your own app](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/both-ai-vendors/): putting the rhythm on a schedule.
- [Lab 3: the same one line](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/lab/): the book's version of this step. The Copperleaf version below replaces it.
- [Check yourself](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

Rosa's problem has a name. A one-line request leaves the worker to guess the intent, the scope, what it may do and what "good" means, so the result depends on its guesses that week. The **10-80-10 rhythm** fixes that. In the **first 10 percent** you make four decisions before the worker starts: intent, scope, authority and the review contract. In the **middle 80** the worker works, and you keep only a small job: watching for a reason to stop it. In the **final 10** you review the evidence, fix each problem where it came from, and a person approves.

When a run goes wrong, the rhythm also tells you where to look: was the first 10 skipped, was the middle 80 micromanaged, or was the final 10 skipped? Naming the failure is the first step to fixing the right thing.

## What you will learn

- The three parts of the rhythm, as a shape rather than a timesheet.
- The four decisions of the first 10 percent.
- What the worker does in the middle 80, and when you interrupt.
- How to review evidence, fix a problem where it came from, and approve.
- The three failures, and the questions that show where to look first.

## What you will make

- `work/one-line-run.md`: the weak run from Ben's one line, and which failure it shows
- `work/first-10.md`: intent, scope, authority and the review contract for the reminder run, written before the run
- `work/rhythm-run/`: the reminder run done in three parts, with the worker's output and its record
- `work/final-10.md`: your evidence review, each problem and where it came from, and the approval
- `work/role-contract.md`: version 2, with its review checks and the reminder run's limits on a schedule
- `NOTES.md`: the proof (the same one line, before and after), and how the apps compared

## Key concepts

- **First 10 percent:** the four decisions made before the worker starts: intent, scope, authority and the review contract.
- **Middle 80 percent:** the worker plans and does the work; the person watches only for a reason to stop it.
- **Final 10 percent:** the person reviews the evidence, fixes each problem where it came from, and approves.
- **Review contract:** how you will know the work is right, agreed before it starts.
- **The three failures:** skipping the first 10, micromanaging the middle 80, and skipping the final 10.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync, start a thread, and bring the contract forward.** Sync your fork, pull in GitHub Desktop, start a new thread for this step, and paste:

```text
I'm doing Step 15 of the bootcamp. Copy step-14-role-contract/work/role-contract.md to step-15-operating-rhythm/work/role-contract.md, unchanged. Don't change step 14's copy. Never commit or push.
```

**2. Ben's one line.** In a fresh ordinary Claude chat (outside your project, see [Finding things in the apps](../step-00-readiness-check/README.md#an-ordinary-chat-outside-the-project)), attach `step-02-three-deliverables/work/claude/figures.csv` and `copperleaf/customers.csv` (not the policy), and type only:

```text
Do this week's reminders.
```

Save what came back in `work/one-line-run.md`. Then, using [3.6](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/three-failures/), write under it which failure it shows, and what the worker had to guess.

**3. The first 10 percent.** Back in your project thread, paste:

```text
Help me write step-15-operating-rhythm/work/first-10.md for the weekly reminder run, using chapter 3.2 of The AI Agent Factory. Ask me about one decision at a time and wait for my answer:
1. Intent: the outcome and why it matters.
2. Scope: what is in, what is out, and which files and policy version it works from.
3. Authority for this task: what the worker may do on its own. It must be within the Role Contract, and may be narrower.
4. Review contract: what must be checked, what evidence comes back, what counts as success, and what makes the worker stop and ask.
Use my words. Never commit or push.
```

Answer in your own words. Then **commit `first-10.md` on its own** in GitHub Desktop (`step-15: first 10 percent`) and push, so it comes before the run in your history.

**4. The middle 80 percent.** Paste:

```text
Do the weekly reminder run as step-15-operating-rhythm/work/first-10.md describes, as of Monday 2 November 2026. Save the reminder list in step-15-operating-rhythm/work/rhythm-run/reminder-list.md and, in step-15-operating-rhythm/work/rhythm-run/record.md, a record of what you did: each file you read, each step, anything you weren't sure of, and anything you stopped for. Draft only. Never commit or push.
```

Don't interrupt unless it is about to break a limit. If you do interrupt, note why in `NOTES.md`.

**5. The final 10 percent.** Review the run against the review contract in `first-10.md`, using the record as your guide. For each problem you find, write in `work/final-10.md`: what it is, where it came from (the brief and first 10, the inputs, or the worker in the middle), and the fix in that place. Then write the approval line: approved, or returned with the fix, by you, with the date.

**6. Draft 2 of the contract.** Paste:

```text
Update step-15-operating-rhythm/work/role-contract.md to Draft 2: add the reminder run's review checks under Evaluations, add the weekly reminder run under Triggers with "drafts only, nothing sent", and add a Change log line: today's date, approved by Rosa (pending), "Draft 2: review checks and the weekly reminder run, from step 15". Change nothing else.
```

**7. The proof: the same one line.** In a fresh thread in your project (which has your instructions and the contract), type `Do this week's reminders.` again, attaching nothing. Compare the result with `one-line-run.md` in `NOTES.md`. What did the project's setup supply that the one line couldn't?

## Repeat it in ChatGPT

1. Do instruction 2's one line in a ChatGPT chat with the same two files, and add the result to `one-line-run.md`.
2. In your ChatGPT project (or, without one, a new chat with the same files attached), attach `first-10.md`, `figures.csv`, `customers.csv` and the policy, and run instruction 4's prompt, downloading its two files into `work/rhythm-run/chatgpt/`.
3. Do the final 10 percent on ChatGPT's run too, in a "ChatGPT" section of `final-10.md`.
4. Look at [3.7](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/both-ai-vendors/), and in `NOTES.md` say how you would put the rhythm on a schedule in each app, and what part of the rhythm a schedule can't do for you.

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **The first 10 came first.** `first-10.md` is in an earlier commit than the run.
- [ ] **Authority is within the contract.** Nothing in `first-10.md` lets the worker do more than the Role Contract allows.
- [ ] **The review contract was used.** `final-10.md` follows its checks, one by one.
- [ ] **The list is right.** Three reminder stages checked by you against policy 5.1; no disputed or paid invoice on it.
- [ ] **Every problem has a home.** Each is fixed where it came from, not patched in the output.
- [ ] **Draft 2 is logged.** The contract's change log has a dated line.

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-15: the rhythm and contract draft 2` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-15-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/one-line-run.md`, with the failure named
- [ ] `work/first-10.md`, committed before the run
- [ ] `work/rhythm-run/` with the list and the record, from Claude and ChatGPT (or a transfer plan in `NOTES.md`)
- [ ] `work/final-10.md` and `work/role-contract.md` (Draft 2)
- [ ] **Checked:** the run reviewed against the review contract, and three reminder stages worked out by you
- [ ] `NOTES.md`: the before-and-after proof, and scheduling in each app
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] `NOTES.md`: one prompt you changed before pasting it, and why
- [ ] Committed, tagged `step-15-done` and pushed

## References

- [Chapter 3: The 10-80-10 Operating Rhythm](https://agentfactory.panaversity.org/ai-worker-paradigm/the-10-80-10-operating-rhythm/overview/)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md), section 5

---

[← Step 14: The Role Contract](../step-14-role-contract/) · [Roadmap](../README.md#roadmap) · [Step 16: The Architecture in One Picture →](../step-16-architecture/)
