# Step 16: The Architecture in One Picture

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Name the parts of a governed AI Worker and decide which ones Copperleaf must own. You draw the Receivables Worker's layers (what knows, what remembers, what tracks where the work stands, what acts, what executes and what connects), mark which layers Copperleaf rents from Anthropic or OpenAI and which knowledge, policies, state and records it owns, and name them in the Role Contract. This step ends milestone 3.

> 🍃 **Copperleaf's ask:** Copperleaf's accountant asked a sharp question: if the AI company changes its product, what does Copperleaf lose? Amira wants a one-page answer.

> ⏱️ **About 5 to 7 hours**, including the reading. Good places to pause: after instruction 4, after instruction 7, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

> 🧭 **Your prompts in this step: Modify.** The prompts are given, but they are a starting point. Before you paste each one, read it and change what doesn't fit what you found in earlier steps (a file name, a check, a limit). In `NOTES.md`, record one prompt you changed, and why.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [4.1 Six layers, six verbs](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/five-layers/): the layers you draw.
- [4.2 KSoR knows](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/ksor-knows/): the governed knowledge Copperleaf owns.
- [4.3 Memory remembers](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/memory-remembers/): what the worker should remember, and which source wins when memory and the record disagree.
- [4.4 SSoR tracks where the work stands](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/ssor-tracks/): where the state of each job is kept.
- [4.5 DSoR acts](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/dsor-acts/): where the worker's power to act is checked.
- [4.6 Rented above, owned below](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/rented-and-owned/): the answer to the accountant's question.
- [4.7 The governance rule](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/governance-rule/): the rule that keeps the worker trustworthy.
- [4.8 Find each layer in your own app](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/both-ai-vendors/): where each layer lives in Claude and in ChatGPT.
- [4.9 Isn't the missing permanent machine a gap?](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/worker-is-the-records/) and [4.10 What changes when others use the worker?](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/when-others-use-it/): two questions the accountant may ask next.
- [Lab 4: what the worker is made of](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/lab/): the book's version of this step. The Copperleaf version below replaces it.
- [Check yourself](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

The book draws every AI Worker with **six layers**, each with one verb. **Channels** connect (where people reach it). The **runtime** executes (the replaceable program that does the work). **Memory** remembers (preferences and experience). The **KSoR** knows (the approved rules). The **SSoR** tracks (one case file for each piece of work, with where it stands). The **DSoR** acts (the governed door to real systems, which checks before acting and keeps the evidence).

The top layers, channels and runtime, are rented from a vendor, and they will change. The records below them must be **owned** by the company: its knowledge, its case files and its evidence. That is the accountant's answer. If Copperleaf owns its records, a product change costs it some setup work. If its rules live only in a vendor's chat history, a product change costs it its memory.

## What you will learn

- The six layers and their verbs, and where the worker itself sits.
- Which layers a company rents and which it must own, and a test that shows where each part really lives.
- Which source wins when memory and the record disagree.
- How the three owned records split governing a worker between them.
- What changes when other people, or another company, use the worker.

## What you will make

- `work/architecture.md`: the one-page map of the Receivables Worker's six layers, what each holds at Copperleaf today, and whether it is rented or owned
- `work/move-test.md`: what Copperleaf would keep and lose if it moved the worker to the other vendor tomorrow
- `work/role-contract.md`: version 3, with its knowledge sources, memory and state named
- `NOTES.md`: your one-page answer for Amira, in your own words
- A recorded project defence, because this step ends milestone 3

## Key concepts

- **Channels (connect):** where people and systems reach the worker: a chat, team messaging, email.
- **Runtime (executes):** the replaceable program, called the harness, that reasons and acts.
- **Memory (remembers):** continuity, such as preferences, experience and where to look. Never the final word on a rule.
- **KSoR (knows):** the Knowledge System of Record: the governed, approved knowledge, such as policies, thresholds and definitions.
- **SSoR (tracks):** the State System of Record: one case file for each piece of work, with where it stands, what was tried and who approved what.
- **DSoR (acts):** the governed door to real systems: it checks, acts, and keeps the evidence.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync, start a thread, and bring the contract forward.** Sync your fork, pull in GitHub Desktop, start a new thread for this step, and paste:

```text
I'm doing Step 16 of the bootcamp. Copy step-15-operating-rhythm/work/role-contract.md to step-16-architecture/work/role-contract.md, unchanged. Never commit or push.
```

**2. Channels and runtime.** Paste:

```text
Using chapter 4.1 of The AI Agent Factory, start step-16-architecture/work/architecture.md with a table of the six layers (channels, runtime, memory, KSoR, SSoR, DSoR), their verbs, and for Copperleaf's Receivables Worker as it is today in this bootcamp: what each layer is, where it lives (which app, which folder, which file), and whether Copperleaf rents it or owns it. Fill in channels and runtime now, and leave the other rows for us to do one at a time. Never commit or push.
```

**3. KSoR: what it knows.** Paste:

```text
Fill in the KSoR row. Where are Copperleaf's approved rules today? Is there one approved copy, with an owner and a date, or several copies? Name every copy you can find in my repo.
```

Check the list yourself: the policy, your step 10 summary, the rules in your project instructions, the skill files from steps 6 and 7. Which one should win?

**4. Memory: what it remembers.** Paste:

```text
Fill in the memory row. What does each app remember about Copperleaf now, and what should the worker be allowed to remember? If memory and the policy disagree, which wins? Use chapter 4.3.
```

Then, in Claude's settings, look at what memory holds (if it is on) and compare.

**5. SSoR: where the work stands.** Paste:

```text
Fill in the SSoR row. Where would the worker look to know where each piece of work stands, for example that PAY-9037 was confirmed by phone, or that INV-4199 is in dispute? Is there one case file per matter today? Use chapter 4.4.
```

(Step 7's `corrections.csv` is a start of one.)

**6. DSoR: the door it acts through.** Paste:

```text
Fill in the DSoR row. Through what does the worker act on real systems today, and what checks happen before an action? Use chapter 4.5, and say honestly how much of this exists in our setup.
```

**7. The move test.** Paste:

```text
Write step-16-architecture/work/move-test.md: if Copperleaf moved the Receivables Worker from this app to the other vendor's tomorrow, what would it keep (because it owns it), what would it lose, and what would it have to set up again? Use chapter 4.6's test. Then answer: what changes when Ben and Rosa, not only I, use the worker (chapter 4.10)?
```

Check every "keep" against your repo: is it really a file Copperleaf owns?

**8. Draft 3 of the contract.** Paste:

```text
Update step-16-architecture/work/role-contract.md to Draft 3: under "What it works with", name the KSoR (the governed source of Copperleaf's rules, and its owner), what Memory may and may not keep, and the case files (SSoR) it reads and writes. Add a Change log line: today's date, approved by Rosa (pending), "Draft 3: knowledge, memory and state named, from step 16". Change nothing else.
```

**9. Write Amira's answer.** In `NOTES.md`, in your own words, answer the accountant's question in under 300 words, using your map and move test.

## Repeat it in ChatGPT

1. Read [4.8](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/both-ai-vendors/), then in your ChatGPT project attach `work/architecture.md` and ask:

   ```text
   Where would each of these six layers live if this worker ran in ChatGPT? Say which settings, features or files hold each one, and which are not available.
   ```
2. Add a "ChatGPT" column to `architecture.md` with the answers you have checked in the app.
3. In `NOTES.md`, say which layers look the same on both vendors, and which differ.

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **Six layers, six verbs,** each with what it is at Copperleaf today and rented or owned.
- [ ] **Every copy of the rules is found,** and one is named as the one that wins.
- [ ] **Memory never wins** over the approved record.
- [ ] **Honest about gaps.** Where a layer doesn't really exist yet (for example, a DSoR), the map says so.
- [ ] **The move test is checked.** Every "keep" is a file in your repo.
- [ ] **Draft 3 is logged** in the contract's change log.

## Record your defence

This step ends milestone 3, so record a project defence of up to five minutes ([SUBMITTING.md, section 10](../SUBMITTING.md#10-defend-your-work)). Show your map; trace one row to the file it names; explain one thing Copperleaf must own and how your setup keeps it owned; and show one change you made to what the AI drafted.

Before you share it, go through the [privacy checklist](../SUBMITTING.md#before-you-share-a-screenshot-or-recording).

## Keep it

Do this last, after the ChatGPT part and your defence. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-16: architecture and contract draft 3` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-16-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/architecture.md`, with Claude and ChatGPT columns (or a transfer plan in `NOTES.md`)
- [ ] `work/move-test.md` and `work/role-contract.md` (Draft 3)
- [ ] **Checked:** every "where it lives" and every "keep" checked by you against your repo and your apps
- [ ] `NOTES.md`: your answer to the accountant's question
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] `NOTES.md`: one prompt you changed before pasting it, and why
- [ ] **Defence:** a link to your recorded project defence, ready for the form
- [ ] Committed, tagged `step-16-done` and pushed

## References

- [Chapter 4: The Architecture in One Picture](https://agentfactory.panaversity.org/ai-worker-paradigm/the-architecture-in-one-picture/overview/)

---

[← Step 15: The 10-80-10 Operating Rhythm](../step-15-operating-rhythm/) · [Roadmap](../README.md#roadmap) · [Step 17: The Four-Part Brief →](../step-17-four-part-brief/)
