# Step 17: The Four-Part Brief

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Brief the Receivables Worker the way Part II teaches: by its outcome, context, format and constraints, naming only the steps that must be followed. You write the brief for the weekly receivables run, name the governed source in its context, break the job into stages with a check between them, fix a weak result by changing only the part of the brief that failed, and compare the runs in Claude and ChatGPT.

> 🍃 **Copperleaf's ask:** Ben, Copperleaf's credit controller, will run the weekly job when you are on leave. Rosa wants a brief that gives Ben the same result you get.

> ⏱️ **About 5 to 7 hours**, including the reading. Good places to pause: after instruction 3, after instruction 5, after instruction 8, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

> 🧭 **Your prompts in this step: Modify.** The prompts are given, but they are a starting point. Before you paste each one, read it and change what doesn't fit what you found in earlier steps (a file name, a check, a limit). In `NOTES.md`, record one prompt you changed, and why.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [Part II: Managing AI Workers](https://agentfactory.panaversity.org/managing-ai-workers/overview/): what this part of the book covers, and its capstone.
- [5.1 Write the brief, part by part](https://agentfactory.panaversity.org/managing-ai-workers/the-four-part-brief/four-parts/): the four parts of the brief.
- [5.2 Iterate: change the part that failed](https://agentfactory.panaversity.org/managing-ai-workers/the-four-part-brief/iterate/): fixing a weak result.
- [5.3 Decompose complex requests](https://agentfactory.panaversity.org/managing-ai-workers/the-four-part-brief/decompose/): stages, with a check between them.
- [5.4 Run the brief in your own app](https://agentfactory.panaversity.org/managing-ai-workers/the-four-part-brief/both-ai-vendors/): running it in both apps.
- [Lab 5: the payment-run brief](https://agentfactory.panaversity.org/managing-ai-workers/the-four-part-brief/lab/): the book's version, on accounts payable. The Copperleaf version below replaces it.
- [Check yourself](https://agentfactory.panaversity.org/managing-ai-workers/the-four-part-brief/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

Part II is about managing a worker, and managing starts with the brief. The book's **Four-Part Brief** has an **outcome** (what exists when the work is done, ending with a "done when" test), a **context** (who it is for, and which source wins when sources disagree), a **format** (the shape the next reader needs) and **constraints** (the content rules, and how far the worker may go alone). It names a step only when the step is a **control**: required by policy, law or a system that uses the result. Everything else is method, and method is the worker's job.

A good brief is also a test. When a result is weak, you can read it against the four parts and find the one that caused the problem, then change only that part. That is how Ben gets your result: not by copying your chat, but by running a brief that leaves nothing to guess.

## What you will learn

- The four parts of a brief, and what each one fixes.
- Which steps belong in a brief (controls) and which don't (method).
- How to name the governed source, so the worker knows which file wins.
- How to read a weak result as a test of the brief, and change only the part that failed.
- How to split a big job into stages, with a stop for a person's decision.

## What you will make

- `work/brief.md`: the Four-Part Brief for the weekly receivables run, with each iteration recorded
- `work/runs/`: the staged run in Claude and in ChatGPT, and a fresh-chat run of the same brief
- `work/iterations.md`: each weak result, the part of the brief that caused it, and the change
- `work/role-contract.md`: version 4, pointing to the brief
- `NOTES.md`: how the two apps compared, and what Ben would need besides the brief

## Key concepts

- **Outcome:** what exists when the work is done, so someone else can tell it's finished, ending with a "done when" sentence.
- **Context:** who the work is for, and which source is the authority when sources disagree.
- **Format:** the shape the result's next reader needs: a table, a file, a memo.
- **Constraints:** the content rules (what the result must keep, leave out or avoid) and the autonomy (how far the worker may go alone).
- **Control:** a step the brief must name because policy, law or a system requires it. Other steps are method, left to the worker.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="../assets/four-part-brief-dark.png">
  <img src="../assets/four-part-brief-light.png" alt="A one-line request leaves the AI to guess. A Four-Part Brief has an outcome (what exists when the work is done, ending with a done-when sentence), context (who it is for, and which source wins when sources disagree), format (the shape the next reader needs) and constraints (content rules and how far the worker may go alone). It also names any control step that policy, law or a system requires; every other step is method, left to the worker." width="100%">
</picture>

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync, start a thread, and bring the contract forward.** Sync your fork, pull in GitHub Desktop, start a new thread for this step, and paste:

```text
I'm doing Step 17 of the bootcamp. Copy step-16-architecture/work/role-contract.md to step-17-four-part-brief/work/role-contract.md, unchanged. Never commit or push.
```

**2. See why the one line fails.** Paste:

```text
Here is how Ben would brief the weekly run today: "Do the Monday receivables run. Everything's in the copperleaf folder." Without running it, list what a worker would have to guess, sorted into the four parts of a brief from chapter 5.1: outcome, context, format and constraints. Then list any steps Ben would add that are really method, not controls.
```

Save the answer at the top of `work/iterations.md` as "Before the brief".

**3. Write the brief, part by part.** Paste:

```text
Help me write step-17-four-part-brief/work/brief.md, a Four-Part Brief for Copperleaf's weekly receivables run, following chapter 5.1. Go one part at a time and wait for me after each:

1. Outcome: what exists when the run is done (the week's payments matched, the open invoices aged, and the reminders due drafted), ending with a "Done when" sentence someone else could test.
2. Context: who it is for (Rosa, and Ben when I'm away), and which source wins: customers.csv for credit limits (policy 3.2), the current policy for every rule, my corrections file from step 7 for confirmed allocations. Name the files that must NOT be used.
3. Format: the files the next readers need, with names and columns.
4. Constraints: the content rules (amounts exactly as recorded, every rule cited by section, nothing guessed) and the autonomy (drafts only; anything outside the policy stops and is listed for a person).

Include a step only if it is a control the policy requires, and say which section. Keep it to one page. Never commit or push.
```

**4. Split it into stages.** Paste:

```text
Using chapter 5.3, add a "Stages" section to brief.md: stage 1, match the payments and list the ones that need a person; STOP for me to check them; stage 2, age the open invoices; stage 3, draft the reminders due. Say what is handed from one stage to the next, and where the stop is.
```

**5. Run it.** In a fresh thread in your project, paste:

```text
Run step-17-four-part-brief/work/brief.md, stage 1 only, as of Monday 2 November 2026. Save the results in step-17-four-part-brief/work/runs/claude/. Then stop.
```

Check stage 1 against your checked step 1 matches. When it's right, reply `Go on to stages 2 and 3.` and check those too, against your step 2 figures and step 15 list.

**6. Change the part that failed.** Look at every weak spot in the run: a missing column, a vague reason, a reminder without a section, a file it shouldn't have read. For each, write in `work/iterations.md`: what was weak, which of the four parts caused it (or whether it was the worker, not the brief), and the one change. Make only that change to `brief.md` and run that stage again. Stop when a run passes, or after three iterations.

**7. Find out why a prompt went generic.** In an ordinary chat (outside your project, see [Finding things in the apps](../step-00-readiness-check/README.md#an-ordinary-chat-outside-the-project)), ask: `Write a reminder to a customer about an overdue invoice.` You will get something generic. In `iterations.md`, say which parts of a brief were missing, then rewrite the request with the four parts and compare.

**8. The proof: a fresh chat.** In a brand-new thread, attach nothing extra and paste only:

```text
Run step-17-four-part-brief/work/brief.md, all stages, as of Monday 2 November 2026, stopping where it says. Save results in step-17-four-part-brief/work/runs/fresh/.
```

Does it give the same result as instruction 5? That is what Ben would get.

**9. Draft 4 of the contract.** Paste:

```text
In step-17-four-part-brief/work/role-contract.md, add the weekly run's brief (work/brief.md) under Procedures, and a Change log line with today's date, approved by Rosa (pending): "Draft 4: weekly run brief, from step 17". Change nothing else.
```

## Repeat it in ChatGPT

1. Read [5.4](https://agentfactory.panaversity.org/managing-ai-workers/the-four-part-brief/both-ai-vendors/) for what the brief must say differently in ChatGPT.
2. In your ChatGPT project (or, without one, a new chat with the same files attached), attach `brief.md` and every file the brief names, and run it stage by stage, stopping where it says. Download the results into `work/runs/chatgpt/`.
3. Compare the two runs in `NOTES.md`, stage by stage. Where they differ, was it the brief (something it left open) or the app?

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **Four parts, one page,** with a "Done when" someone else could test.
- [ ] **The governed source is named,** and the stale file is named as one not to use.
- [ ] **Every step in the brief is a control,** with its policy section.
- [ ] **The stop is real.** Stage 1 stopped for you before stage 2.
- [ ] **The results are right.** Stage 1 matches your checked step 1 matches; stage 2's total matches your step 2 total.
- [ ] **Each iteration changed one part,** and `iterations.md` says which.
- [ ] **The fresh chat matched.** Or, where it didn't, you found which part of the brief left it room to differ.

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-17: four-part brief` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-17-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/brief.md`, with its stages
- [ ] `work/iterations.md`, including "Before the brief" and the generic-prompt test
- [ ] `work/runs/` with Claude's run, the fresh run and ChatGPT's run (or a transfer plan in `NOTES.md`)
- [ ] `work/role-contract.md` (Draft 4)
- [ ] **Checked:** stage 1 and stage 2 results compared by you with your checked figures from steps 1 and 2
- [ ] `NOTES.md`: how the apps compared, and what Ben would need besides the brief
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] `NOTES.md`: one prompt you changed before pasting it, and why
- [ ] Committed, tagged `step-17-done` and pushed

## References

- [Chapter 5: The Four-Part Brief](https://agentfactory.panaversity.org/managing-ai-workers/the-four-part-brief/overview/)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md)

---

[← Step 16: The Architecture in One Picture](../step-16-architecture/) · [Roadmap](../README.md#roadmap) · [Step 18: The Review Contract →](../step-18-review-contract/)
