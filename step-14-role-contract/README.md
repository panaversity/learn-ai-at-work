# Step 14: The Role Contract

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Describe the AI Worker that Copperleaf needs as a role, not a tool. You write the first one-page Role Contract for Copperleaf's Receivables Worker: its mission, its responsibilities, its authority, its tools, the knowledge it uses, and the person accountable for it. You will refine this contract in almost every step that follows.

> 🍃 **Copperleaf's ask:** Rosa is willing to give an AI Worker part of her team's receivables work. Before she does, she wants it written down like a job description: what it does, what it may not do, and who answers for it.

> ⏱️ **About 4 to 6 hours**, including the reading. Good places to pause: after instruction 3, after instruction 4, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

> 🧭 **Your prompts in this step: Modify.** The prompts are given, but they are a starting point. Before you paste each one, read it and change what doesn't fit what you found in earlier steps (a file name, a check, a limit). In `NOTES.md`, record one prompt you changed, and why.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [2.1 The anatomy of an AI Worker](https://agentfactory.panaversity.org/ai-worker-paradigm/what-is-an-ai-worker/anatomy-of-an-ai-worker/): the parts every Role Contract names.
- [2.2 Five things people call "AI"](https://agentfactory.panaversity.org/ai-worker-paradigm/what-is-an-ai-worker/five-things-called-ai/): a worker versus a model, agent, assistant or automation.
- [2.3 Worker, runtime and channel](https://agentfactory.panaversity.org/ai-worker-paradigm/what-is-an-ai-worker/worker-runtime-channel/): what runs the worker and where people reach it.
- [2.4 Choosing a surface and a model](https://agentfactory.panaversity.org/ai-worker-paradigm/what-is-an-ai-worker/surface-and-model/): choosing where Copperleaf's worker runs, and when to use a project, a skill, research or code.
- [2.5 Choose what runs it, in your own app](https://agentfactory.panaversity.org/ai-worker-paradigm/what-is-an-ai-worker/both-ai-vendors/): where the worker would run in Claude and in ChatGPT.
- [2.6 The Role Contract](https://agentfactory.panaversity.org/ai-worker-paradigm/what-is-an-ai-worker/role-contract/): the document you write.
- [Lab 2: the first Role Contract](https://agentfactory.panaversity.org/ai-worker-paradigm/what-is-an-ai-worker/lab/): the book's version of this step. The Copperleaf version below replaces it.
- [Check yourself](https://agentfactory.panaversity.org/ai-worker-paradigm/what-is-an-ai-worker/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

An **AI Worker** is not a model, an app or an automation. It is a role: a defined piece of a team's work, held over time, inside limits, with a named person who answers for it. The model and the app that run it can change; the role shouldn't. That is why the book writes a worker down as a **Role Contract**: a one-page definition that is portable (it would work on another vendor's app), owned (by Copperleaf, not the vendor) and checkable (every line can be tested).

From this step on, the Receivables Worker is the thread through the rest of the bootcamp. Each Part II chapter fills in one part of its contract: the brief, the checks, the authority, the knowledge, the triggers, the governance and the change log.

## What you will learn

- The sixteen elements that define an AI Worker, in five groups.
- How a worker differs from a model, an assistant, an automation and an agent.
- Why a worker is defined apart from the runtime that runs it and the channels people reach it through.
- How to choose a surface, the features the work needs (a project, a skill, research or code) and a model.
- How to write a first Role Contract, and test it.

## What you will make

- `work/role-contract.md`: the first draft of the Role Contract for Copperleaf's Receivables Worker
- `work/feature-choices.md`: for each of the worker's jobs, whether it needs a project, a skill, research or code, and why
- `work/contract-test.md`: the final test of the draft, and what you changed
- `NOTES.md`: the open questions you would put to Rosa, and how the two apps compared

## Key concepts

- **AI Worker:** an AI that holds a role and does the same work again and again, inside limits a person sets, with a named owner.
- **Role Contract:** a worker's portable, owned and checkable one-page definition.
- **Runtime:** the replaceable program that runs the worker's work.
- **Channel:** where people and systems reach the worker, such as a chat or an inbox.
- **Delegated or standing:** a delegated worker does each job from a brief; a standing worker holds an ongoing role that its triggers start.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync and start a thread.** Sync your fork, pull in GitHub Desktop, and start a new thread for this step.

**2. Tell it apart.** Paste:

```text
I'm doing Step 14 of the bootcamp. Using chapter 2.2 of The AI Agent Factory, quiz me with five short Copperleaf examples, one at a time, and ask whether each is a model, an assistant, an automation, an agent or an AI Worker. After each answer, tell me in one line if I'm right and why.
```

**3. Gather what the worker will do.** Paste:

```text
From everything in steps 1 to 13 of this bootcamp (the work folders in my repo) and copperleaf/policies/credit-and-collections-policy.md, list the receivables work an AI Worker at Copperleaf could hold: each recurring job, how often, what it reads, what it produces, and where the result is kept. Mark any job the policy keeps for a person, with the section. Don't write anything yet.
```

**4. Write the contract, one group at a time.** Paste:

```text
Now help me write step-14-role-contract/work/role-contract.md, Draft 1, using the template in chapter 2.6 of The AI Agent Factory, with its six headings: Who it is, What it owes, What it works with, What bounds it, How it runs and is reached, Open questions.

Go one heading at a time. For each, propose the lines, then ask me to confirm or change them before you go on. Use what we found in this thread. The worker is "Copperleaf Receivables Worker"; its owner is Rosa, Finance Manager. In "What bounds it", give every action one of: observe, recommend, draft, execute, escalate or never, and nothing that sends to a customer or changes bank details may be above draft. Leave the Change log empty. Keep it to one page. Never commit or push.
```

Answer each heading in your own words. If you don't know something yet (how it will be evaluated, for example), put it under Open questions; later steps answer them.

**5. Choose the features.** Paste:

```text
Make step-14-role-contract/work/feature-choices.md: for each job in the contract's Responsibilities, which features it needs (a project, a skill, research, code execution, a connector, a scheduled task) and which it doesn't, with one line why, using chapter 2.4's rules. Then fill in "Runtime needs" in the contract: the surface, how it keeps going between runs, and the model and effort, with today's date.
```

Check each choice against [2.4](https://agentfactory.panaversity.org/ai-worker-paradigm/what-is-an-ai-worker/surface-and-model/).

**6. The final test.** Paste:

```text
Test the Role Contract with the four checks for a first draft in chapter 2.6. For each check, say pass or fail and quote the line. Then answer: could someone else run this worker on another vendor's app using only this page? Write the results in step-14-role-contract/work/contract-test.md. Don't change the contract.
```

Fix what failed (ask Claude to change only those lines), and note each change in `contract-test.md`.

## Repeat it in ChatGPT

1. In your ChatGPT project (or, without one, a new chat with the same files attached), attach `work/role-contract.md` and the policy, and paste:

```text
Read this Role Contract for an AI Worker as if you had to run the worker tomorrow. List every line that is unclear, every action whose limit isn't stated, and anything the policy requires that the contract leaves out. Then say where this worker would run in ChatGPT, and what in the contract would need to change to run it there.
```

2. Save the answer as `work/chatgpt-contract-review.md`, mark each point *accepted* or *rejected*, and make the accepted changes in Claude.

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **All six headings** of the book's template, on one page.
- [ ] **A named owner:** Rosa, Finance Manager.
- [ ] **Every action has a rung,** and nothing that sends, pays or changes bank details is above draft (policy 5.3, 8.3, 9).
- [ ] **The policy's "person only" jobs stay with people.** Check each against section 11.
- [ ] **Runtime needs are dated,** because the products will change.
- [ ] **Portable:** nothing in the contract only makes sense in one vendor's app.

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-14: Role Contract draft 1` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-14-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/role-contract.md`, Draft 1
- [ ] `work/feature-choices.md` and `work/contract-test.md`
- [ ] `work/chatgpt-contract-review.md` (or a transfer plan in `NOTES.md`)
- [ ] **Checked:** every rung and every "person only" job checked by you against policy section 11
- [ ] `NOTES.md`: your open questions for Rosa, and how the apps compared
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] `NOTES.md`: one prompt you changed before pasting it, and why
- [ ] Committed, tagged `step-14-done` and pushed

## References

- [Chapter 2: What Is an AI Worker?](https://agentfactory.panaversity.org/ai-worker-paradigm/what-is-an-ai-worker/overview/)
- [2.6 The Role Contract](https://agentfactory.panaversity.org/ai-worker-paradigm/what-is-an-ai-worker/role-contract/)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md), section 11

---

[← Step 13: From Chatbots to AI Workers](../step-13-chatbots-to-ai-workers/) · [Roadmap](../README.md#roadmap) · [Step 15: The 10-80-10 Operating Rhythm →](../step-15-operating-rhythm/)
