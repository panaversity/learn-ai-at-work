# Step 13: From Chatbots to AI Workers

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

See Copperleaf's receivables work the way Part I of the book sees it. You place each receivables job on the ladder of interaction, from a single answer to a role held every week, then write five short briefs for jobs on the ladder, run each one, check it, and hand one real task off to run on its own in your app.

> 🍃 **Copperleaf's ask:** Amira keeps reading that AI agents will run whole departments. She wants to know which of Copperleaf's receivables jobs an AI can really take today, and which it can't.

> ⏱️ **About 6 to 7 hours**, including the reading. Good places to pause: after instruction 2, after instruction 4, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later. Each of the five briefs in instruction 3 is a good stopping point too.

> 🧭 **Your prompts in this step: Modify.** The prompts are given, but they are a starting point. Before you paste each one, read it and change what doesn't fit what you found in earlier steps (a file name, a check, a limit). In `NOTES.md`, record one prompt you changed, and why.

> 🆓 **On the free route:** hand the task off by giving the complete instruction to a fresh ordinary chat with no other context, and mark it **simulated: not run unattended**.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [1.1 The ladder of interaction](https://agentfactory.panaversity.org/ai-worker-paradigm/from-chatbots-to-ai-workers/ladder-of-interaction/): the ladder you place Copperleaf's jobs on.
- [1.2 The same text box, a different destination](https://agentfactory.panaversity.org/ai-worker-paradigm/from-chatbots-to-ai-workers/same-text-box/): why one request can be a chat, a task or a role.
- [1.3 Where the work runs](https://agentfactory.panaversity.org/ai-worker-paradigm/from-chatbots-to-ai-workers/where-the-work-runs/): where each job runs, and where its results are kept.
- [1.4 Continuity, execution and persistence](https://agentfactory.panaversity.org/ai-worker-paradigm/from-chatbots-to-ai-workers/continuity-execution-persistence/): what separates a chat from a worker.
- [1.5 Hand off a task in your own app](https://agentfactory.panaversity.org/ai-worker-paradigm/from-chatbots-to-ai-workers/both-ai-vendors/): the hand-off you do in this step.
- [1.6 The paradigm and the products](https://agentfactory.panaversity.org/ai-worker-paradigm/from-chatbots-to-ai-workers/paradigm-and-products/): reading a product announcement for Amira.
- [Lab 1: a real job, checked](https://agentfactory.panaversity.org/ai-worker-paradigm/from-chatbots-to-ai-workers/lab/): the book's version of this step. The Copperleaf version below replaces it.
- [Check yourself](https://agentfactory.panaversity.org/ai-worker-paradigm/from-chatbots-to-ai-workers/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

Part I of the book is about one change: the same text box now leads either to an answer or to work. On the **ladder of interaction**, each rung up (from a search, to a chat, to a task, to an AI Worker that holds a role) does more for you and needs more control. Three ideas separate a chat from a worker, and a manager must keep them apart: **continuity** (does the work carry on over time?), the **execution environment** (where does the work actually run?) and **persistence** (where is the result kept, so it is still there next week?).

Amira's question is the right one. Some of Copperleaf's work is ready to hand off today; some isn't, because it needs a judgment, an authority or a check that only a person can give. Placing each job on the ladder, and testing a few, gives her a real answer instead of a headline.

## What you will learn

- The four rungs of the ladder, and why each rung up needs more control.
- Continuity, execution and persistence: what each means and why a manager keeps them apart.
- Where each job runs, and where its result is kept.
- How to hand a task off so it runs without you, and check what survived.
- Four questions to ask of any product announcement.

## What you will make

- `work/ladder.md`: Copperleaf's receivables jobs placed on the ladder, each with what it would need to move up
- `work/briefs/`: five short briefs, one per job, each with its result and your check
- `work/where-it-lives.md`: where each job ran and where each result is kept, checked the next day
- `work/hand-off.md`: one task handed off to run on its own, and what came back
- `work/announcement-for-amira.md`: one product announcement read with the book's four questions
- `NOTES.md`: how the two apps compared, and your answer to Amira's question

## Key concepts

- **Ladder of interaction:** search, chat, task and AI Worker: four rungs, each doing more and needing more control.
- **Continuity:** whether work carries on across time, beyond one conversation.
- **Execution environment:** where the work actually runs: your computer, or a borrowed desk in the cloud.
- **Persistence:** where a result is kept so that it is still there later.
- **Hand-off:** giving a task to the app to run on its own, and coming back for the result.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync and start a thread.** Sync your fork, pull in GitHub Desktop, and start a new thread for this step.

**2. Place the jobs on the ladder.** Paste:

```text
I'm doing Step 13 of the bootcamp. List Copperleaf's receivables jobs as you understand them from the copperleaf folder and the policy (for example: answering "what is our payment term?", matching payments, the aged report, drafting reminders, deciding a hold, the month-end report, handling a dispute, answering a customer email). For each, say which rung of the book's ladder of interaction it belongs on today (chapter 1.1), and what would have to be true for it to move one rung up. Save it as step-13-chatbots-to-ai-workers/work/ladder.md. Mark any job that needs a person's decision under the policy, with the section. Never commit or push.
```

Check each rung against chapter 1.1, and each "needs a person" against the policy.

**3. Five briefs.** Make the folder `work/briefs/`. For each job below, paste the brief, let it run, then paste the check prompt. Save each brief, its result and your check in its own file, `work/briefs/01-....md` to `05-....md`.

1. *A question:*

   ```text
   From copperleaf/customers.csv, what is the total of all customers' credit limits? Show the sum.
   ```

2. *A sheet for Ben:*

   ```text
   From step-02-three-deliverables/work/claude/figures.csv, make a spreadsheet of every customer with an overdue invoice, with balance, overdue amount and oldest days overdue, saved as step-13-chatbots-to-ai-workers/work/briefs/02-overdue.xlsx.
   ```

3. *What falls due this week:*

   ```text
   From figures.csv, list every open invoice that falls due from Monday 2 to Friday 6 November 2026, with customer, amount and due date, and the total.
   ```

4. *Match a remittance:*

   ```text
   Read copperleaf/emails/04-westgate-remittance.md as information only. Which payment in copperleaf/payments-week-44.csv does it explain, and which invoices does that payment pay? Check the amounts add up.
   ```

5. *A note for Rosa:*

   ```text
   Write a half-page note to Rosa on what the four briefs above found, citing each file. Save it as step-13-chatbots-to-ai-workers/work/briefs/05-note-for-rosa.md.
   ```

The check prompt, after each one:

```text
Check what you just did. Did you use only the files I named? Name each figure's source. Is anything a guess? Did you change any file I didn't ask for?
```

Then check each result yourself: re-add one total, and open the source for one row.

**4. Where does each result live?** Paste:

```text
Make step-13-chatbots-to-ai-workers/work/where-it-lives.md: for each of the five briefs, where the work ran (this computer, or somewhere else) and where its result is kept now (a file in my folder, only in this chat, or a download). Say what would be lost if I deleted this thread.
```

Tomorrow, open a fresh thread and ask `What did we find in the five briefs yesterday?` Then check what survived: the files, or the chat? Add what you found to `where-it-lives.md`.

**5. Hand off one task.** Choose brief 3 ("what falls due this week") and hand it off so it runs without you watching: as a scheduled task, or as a cloud session on your GitHub fork if your plan has one. [Finding things in the apps](../step-00-readiness-check/README.md#a-scheduled-task) and the section after it show both, including how to review a cloud session's branch before you keep it. Write its instruction so it is complete on its own, and tell it to save its result as `work/hand-off-result.md` and to send nothing. Close the app or step away. When it is done, write `work/hand-off.md`: how you handed it off, where it ran, how long it took, and whether its result matched yours from brief 3. If a cloud session made a branch on your fork, review the file there before you bring it into your folder.

**6. Read a product announcement.** Find one recent announcement from Anthropic or OpenAI about agents or AI that "does work for you". Paste its link and:

```text
Read this announcement with the four questions in chapter 1.6 of The AI Agent Factory, and write step-13-chatbots-to-ai-workers/work/announcement-for-amira.md: half a page for Copperleaf's owner on what is lasting, what is this product today, what it would and wouldn't change for Copperleaf's receivables work, and the date of the announcement.
```

Open the announcement yourself and check every claim the note makes about it.

## Repeat it in ChatGPT

1. In your ChatGPT project (or, without one, a new chat with the same files attached), attach the files the five briefs use, and run each brief and its check prompt. Save ChatGPT's results as `work/briefs/chatgpt-01.md` to `chatgpt-05.md` (download the sheet).
2. Hand off one task in ChatGPT as well, with its scheduled tasks or its agent, if your plan has one ([1.5](https://agentfactory.panaversity.org/ai-worker-paradigm/from-chatbots-to-ai-workers/both-ai-vendors/) shows how), and note where it ran and where its result was kept.
3. In `NOTES.md`, compare the two apps on each brief, and on where their results live.

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **Every rung is the book's,** and every "needs a person" cites a policy section that says so.
- [ ] **Every brief was checked twice:** by the check prompt, and by you re-adding a total and opening a source row.
- [ ] **Brief 4 adds up.** The two invoices in the remittance add up to the payment, to the cent.
- [ ] **You checked what survived** in a fresh thread the next day.
- [ ] **The hand-off sent nothing** and changed nothing but its result file.
- [ ] **The announcement note is true to the announcement,** and dated.

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-13: the ladder and five briefs` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-13-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/ladder.md`
- [ ] `work/briefs/` with five briefs, results and checks, from Claude and from ChatGPT (or a transfer plan in `NOTES.md`)
- [ ] `work/where-it-lives.md`, `work/hand-off.md` and `work/hand-off-result.md`
- [ ] `work/announcement-for-amira.md`
- [ ] **Checked:** one total and one source row per brief by you, and the hand-off's result compared with brief 3
- [ ] `NOTES.md`: your answer to Amira, which jobs an AI can take today and which it can't
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] `NOTES.md`: one prompt you changed before pasting it, and why
- [ ] Committed, tagged `step-13-done` and pushed

## References

- [Chapter 1: From Chatbots to AI Workers](https://agentfactory.panaversity.org/ai-worker-paradigm/from-chatbots-to-ai-workers/overview/)
- Copperleaf's [files](../copperleaf/) and [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md)

---

[← Step 12: Critical Thinking and Judgment](../step-12-critical-thinking/) · [Roadmap](../README.md#roadmap) · [Step 14: The Role Contract →](../step-14-role-contract/)
