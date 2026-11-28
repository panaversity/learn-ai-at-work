# Step 20: Context, Memory, Knowledge and State

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Give the Receivables Worker one authoritative source for Copperleaf's policies. You write five of Copperleaf's receivables policies (payment terms, credit limits and holds, the reminder schedule, disputes and credit notes, and write-off approval) as approved concepts, each with an owner, an approval status and dates, load them into a project in Claude and in ChatGPT, and test where each answer comes from. In one app you also give the project the concepts through a connector (for example, a Google Drive folder) instead of an upload, and you review, edit and delete what the app's memory holds about Copperleaf, and try an incognito chat to see what it knows without memory. This step ends milestone 4.

> 🍃 **Copperleaf's ask:** Copperleaf changed its payment terms from 45 to 30 days in March, but the AI still quotes the old ones. Rosa wants one place where policy is official, and a way to know every copy is current.

> ⏱️ **About 7 to 9 hours**, including the reading. Good places to pause: after instruction 4, after instruction 6, after instruction 8, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

> 🧭 **Your prompts in this step: Modify.** The prompts are given, but they are a starting point. Before you paste each one, read it and change what doesn't fit what you found in earlier steps (a file name, a check, a limit). In `NOTES.md`, record one prompt you changed, and why.

> 🆓 **On the free route:** you can't make a separate project or a connector. Put the five concepts in one zip, attach only that zip to a fresh ordinary chat with the project instructions pasted first, run the tests there, and mark the setup **simulated** in `project-setup.md`. Memory and incognito work on free plans.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [8.1 Five places an answer comes from](https://agentfactory.panaversity.org/managing-ai-workers/context-memory-knowledge-and-state/five-places/): context, memory, knowledge, state and the model.
- [8.2 Context, memory and the case file](https://agentfactory.panaversity.org/managing-ai-workers/context-memory-knowledge-and-state/context-window/): when to restart, summarize or persist.
- [8.3 The workspace and the official record](https://agentfactory.panaversity.org/managing-ai-workers/context-memory-knowledge-and-state/configure-the-workspace/): the KSoR you build.
- [8.4 Set up the project in your own app](https://agentfactory.panaversity.org/managing-ai-workers/context-memory-knowledge-and-state/both-ai-vendors/): loading it into both apps.
- [8.5 Skills and plugins: who approved the steps?](https://agentfactory.panaversity.org/managing-ai-workers/context-memory-knowledge-and-state/skills-and-plugins/): approving the steps a skill adds.
- [Lab 8: where each answer comes from](https://agentfactory.panaversity.org/managing-ai-workers/context-memory-knowledge-and-state/lab/): the book's version of this step. The Copperleaf version below replaces it.
- [Check yourself](https://agentfactory.panaversity.org/managing-ai-workers/context-memory-knowledge-and-state/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

Every answer the worker gives comes from one of five places: the **context** in front of it, its **memory**, the **knowledge** it was given, the **state** of the work, or the **model**'s training. For a question about a rule, only one of those may decide: the approved knowledge. When an old copy of a rule sits in memory, in a chat or in a forgotten file, the worker may quote it, sure-voiced, as Rosa found with the old 45-day terms.

The book's answer is a **KSoR**: each rule written once, as a **concept** with an owner and a status. A concept starts as a *draft*, becomes *stable* only when an authorized person approves it, and becomes *deprecated*, pointing to its successor, when replaced. Only stable concepts in force are served. When the record doesn't cover a question, the right answer is "the record does not say". Then you load that record into each app's project, remove what competes with it, and check what memory holds.

## What you will learn

- The five places an answer can come from, and which may decide a question about a rule.
- When to restart, summarise or persist a long conversation, and what memory may keep.
- How to write rules as KSoR concepts with an owner, a status and dates.
- How to load a project with only approved knowledge, by upload or through a connector.
- How to review, edit and delete memories, and what an incognito chat knows.
- How to approve a skill, and how one change reaches every copy.

## What you will make

- `work/ksor/`: five approved receivables concepts, each with owner, status, version and dates
- `work/project-setup.md`: what each app's project loads, its instructions, and the version of the concepts it holds
- `work/where-from-test.md`: the where-did-this-come-from test in both apps
- `work/memory-and-sources.md`: which source you uploaded and which you connected, and why; what memory held, what you edited or deleted, and what the incognito chat knew (the book's [Lab 8, Task 3](https://agentfactory.panaversity.org/managing-ai-workers/context-memory-knowledge-and-state/lab/#task-3-what-memory-may-keep) and [Task 12](https://agentfactory.panaversity.org/managing-ai-workers/context-memory-knowledge-and-state/lab/#task-12-what-it-holds-and-reaches))
- `work/role-contract.md`: version 7, with the KSoR as its knowledge source
- `NOTES.md`: how the apps compared
- A recorded project defence, because this step ends milestone 4

## Key concepts

- **Five places:** context, memory, knowledge, state and the model's training; each kind of fact has one place that is final.
- **KSoR concept:** one rule, written once, in a short Markdown file whose header says its owner, status, source, approval and dates.
- **Draft, stable, deprecated:** a concept's status: being written; approved and served; replaced, with a pointer to its successor.
- **Abstention:** answering "the record does not say" when the knowledge doesn't cover a question.
- **Projection:** a copy of approved knowledge loaded somewhere else, such as a project. Every copy must say which version it holds.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync, start a thread, and bring the living documents forward.** Sync your fork, pull in GitHub Desktop, start a new thread for this step, and paste:

```text
I'm doing Step 20 of the bootcamp. Copy step-19-authority-envelope/work/role-contract.md, brief.md, review-contract.md and authority-envelope.md to step-20-knowledge-and-state/work/, unchanged. Never commit or push.
```

**2. Four wrong answers: where did each come from?** In an ordinary chat, with no files, ask: `What are Copperleaf Supply's payment terms?`, `When does Copperleaf put an account on hold?`, `Who approves a credit note of 1,800 at Copperleaf?` and `What is The Lantern Room's credit limit?` For each answer, write in `work/where-from-test.md` which of the five places it came from ([8.1](https://agentfactory.panaversity.org/managing-ai-workers/context-memory-knowledge-and-state/five-places/)), and whether it was right.

**3. Write the five concepts.** Paste:

```text
Using chapter 8.3 of The AI Agent Factory, split copperleaf/policies/credit-and-collections-policy.md (version 4.0) into five KSoR concepts, one topic each, saved in step-20-knowledge-and-state/work/ksor/:
payment-terms.md, credit-limits-and-holds.md, reminder-schedule.md, disputes-and-credit-notes.md, write-off-approval.md.

Each file starts with a header between --- lines, with: type (Policy), title, status (draft), version (1), source (the policy version and sections), owner (Rosa, Finance Manager), approval (empty for now), effective_from (the policy's effective date), stale_after (the policy's next review), audience (finance-team). Below the header, the rule in plain words, with every number and condition exactly as the policy says and each sentence citing its section. Nothing from Appendix A. Never commit or push.
```

Check every concept line by line against the policy, as you did in step 10.

**4. Approve them.** For each concept you have checked, change `status: draft` to `status: stable` and fill in `approval` with `Rosa, Finance Manager, <today's date>` (ask Claude to do it, naming each file). A concept you haven't checked stays a draft.

**5. Set up the project with only approved knowledge.** Following [8.4](https://agentfactory.panaversity.org/managing-ai-workers/context-memory-knowledge-and-state/both-ai-vendors/), create a new Claude project, `Copperleaf Receivables Worker`, so the worker's knowledge is separate from your bootcamp project. Add the five stable concepts to its knowledge, and nothing that competes with them (no old summaries, no archive). Give it instructions:

```text
You are Copperleaf's Receivables Worker. Answer questions about Copperleaf's rules only from the five approved concepts in this project's knowledge, and cite the concept and its version. If they don't cover a question, say "The record does not say" and name who to ask (Rosa). Never use rules from memory or general knowledge. Draft only; never send.
```

Add the step 7 month-end skill too, if it's approved, so the project has instructions, knowledge and a skill for a recurring task. Write what the project loads, and the concepts' version, in `work/project-setup.md`.

**6. Test where each answer comes from.** In the new project, ask the four questions from instruction 2 again, plus one the record doesn't cover (`What is Copperleaf's policy on cash discounts for early payment?`). Add the answers to `where-from-test.md`. Each should cite a concept, or abstain.

**7. Memory.** In Claude, open **Settings** and find memory ([Finding things in the apps](../step-00-readiness-check/README.md#memory) has the path in each app). Look at what it holds about Copperleaf. Delete anything that states a Copperleaf rule (rules belong in the KSoR, not memory), and edit anything that is wrong. Then open an incognito chat and ask `What are Copperleaf's payment terms?` Write all of it in `work/memory-and-sources.md`.

**8. One change, every copy.** Pretend Rosa changes the 7-day reminder to 10 days. Make the change as the book does: a new version of `reminder-schedule.md` (version 2, a new approval), the old one marked `deprecated` with a pointer to the new one. Then list every copy that must be refreshed: the project's knowledge, your step 10 summary, the skill from step 6, your project instructions. Refresh the project's copy and test it. Then **change it back** to version 1's rule as a version 3 (this is practice: the policy hasn't really changed), and note it all in `project-setup.md`.

**9. Draft 7 of the contract.** Paste:

```text
In step-20-knowledge-and-state/work/role-contract.md, name the five KSoR concepts in work/ksor/ as the Knowledge sources, with their owner and approver, and add a Change log line with today's date, approved by Rosa (pending): "Draft 7: KSoR, from step 20". Change nothing else.
```

## Repeat it in ChatGPT

1. In ChatGPT, create a project `Copperleaf Receivables Worker`, give it the same instructions, and give it the five stable concepts **through a connector** instead of an upload: put them in a folder in your own Google Drive (or OneDrive) and connect it ([8.4](https://agentfactory.panaversity.org/managing-ai-workers/context-memory-knowledge-and-state/both-ai-vendors/) shows how). If your plan has no connectors, upload them and say so.
2. Ask the same five questions, and add the answers to `where-from-test.md`.
3. Review ChatGPT's memory (in its settings), delete or edit as in instruction 7, and ask the payment-terms question in a Temporary Chat.
4. In `work/memory-and-sources.md`, say which source you uploaded and which you connected, and when each is the better route: for example, a connector stays current when the file changes, and an upload is a copy that can go stale.

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **Five concepts, one topic each,** every line checked by you against the policy, and nothing from Appendix A.
- [ ] **Only checked concepts are stable,** each with an approval and dates.
- [ ] **The project holds nothing that competes.** No archive file, no old summaries.
- [ ] **Every answer cites a concept, or abstains,** in both apps.
- [ ] **The Lantern Room's limit** in the answer is the one in `customers.csv`. Check it yourself.
- [ ] **No rule lives in memory.** You looked, and deleted any.
- [ ] **The change reached every copy,** and was put back.

## Record your defence

This step ends milestone 4, so record a project defence of up to five minutes ([SUBMITTING.md, section 10](../SUBMITTING.md#10-defend-your-work)). Show the project answering from the KSoR; trace one answer to its concept and the policy section; explain one decision about what stays out of the project or out of memory; and show one change you made to a concept the AI drafted.

Before you share it, go through the [privacy checklist](../SUBMITTING.md#before-you-share-a-screenshot-or-recording).

## Keep it

Do this last, after the ChatGPT part and your defence. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-20: KSoR and project setup` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-20-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/ksor/` with five concepts (and the version history of `reminder-schedule.md`)
- [ ] `work/project-setup.md`, `work/where-from-test.md` and `work/memory-and-sources.md`, for both apps (or a transfer plan in `NOTES.md`)
- [ ] `work/role-contract.md` (Draft 7)
- [ ] **Checked:** every concept compared with the policy by you, and every test answer checked against its concept
- [ ] `NOTES.md`: how the apps compared
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] `NOTES.md`: one prompt you changed before pasting it, and why
- [ ] **Defence:** a link to your recorded project defence, ready for the form
- [ ] Committed, tagged `step-20-done` and pushed

## References

- [Chapter 8: Context, Memory, Knowledge and State](https://agentfactory.panaversity.org/managing-ai-workers/context-memory-knowledge-and-state/overview/)
- [Projects in ChatGPT](https://help.openai.com/en/articles/10169521-projects-in-chatgpt) (OpenAI)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md) and [customer list](../copperleaf/customers.csv)

---

[← Step 19: The Authority Envelope](../step-19-authority-envelope/) · [Roadmap](../README.md#roadmap) · [Step 21: Work That Runs Without You →](../step-21-recurring-work/)
