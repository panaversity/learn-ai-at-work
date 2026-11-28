# Step 05: An Overnight Job for a Client

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Follow Nisha's first paid job in the book's second case, and hand over a bigger job to run while you are away. Overnight, the AI prepares a statement and a draft reminder for every Copperleaf customer with an overdue invoice. In the morning you check every amount and every reminder against the ledger and the policy before anything is used, and nothing is sent.

> 🍃 **Copperleaf's ask:** Copperleaf's quarter-end letters to overdue customers take Rosa's team three days. She wants them drafted overnight, but she will not accept a letter nobody checked.

> ⏱️ **About 6 to 7 hours**, including the reading. Good places to pause: after instruction 4, after instruction 5, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later. Instruction 4 is a natural overnight pause: start the run in the evening and check it in the morning.

> 🆓 **On the free route:** start the job in an ordinary chat in the evening instead of a scheduled task, mark the pack **simulated: not run unattended**, and do the morning check exactly as written.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [Case 2: Nisha's First Client](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-2-nishas-first-client/overview/): the case this step follows.
- [A paid job](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-2-nishas-first-client/a-paid-job/): what changes when the work is for someone else.
- [Building the AI Worker](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-2-nishas-first-client/building-the-ai-worker/): setting up a job that runs overnight.
- [Thursday night](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-2-nishas-first-client/thursday-night/): what happens when nobody is watching.
- [Lab: run Nisha's first client job](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-2-nishas-first-client/lab-run-nishas-first-client-job/): the book's version of the overnight job. The Copperleaf job below replaces it.
- [Final assessment: a new AI Worker](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-2-nishas-first-client/final-assessment-a-new-ai-worker/): the assessment you answer at the end.
- [Exhibits](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-2-nishas-first-client/exhibits/): the case's documents.
- [Questions for discussion](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-2-nishas-first-client/questions-for-discussion/): the questions you answer in your notes.
- [Check yourself](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-2-nishas-first-client/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

So far you watched every job. A job that runs overnight is different: nobody is there to notice a wrong turn, and by morning there may be twenty letters, each one plausible. Nisha's lesson from her first client is that the work you do **before** the run (one clear brief, locked limits, a tested lock) and **after** it (a morning check of every item) is what makes overnight work safe. The run in the middle is the easy part.

Letters to customers raise the stakes. Each one states an amount a customer owes, so each one must be right, must follow the reminder schedule, and must go out only after a person signs.

## What you will learn

- How to write a brief once, so a run nobody watches has everything it needs.
- How to lock what matters, and test the lock before the run.
- What standing instructions do, and what memory does, and why a nightly job should rely on instructions.
- How to check a large batch of output, item by item, in the morning.
- Why the person who releases the work is not the AI that made it.

## What you will make

- `work/brief.md`: the brief for the overnight job, written once
- `work/statement-pack/`: one statement and, where the schedule calls for one, one draft reminder for each customer with an overdue invoice
- `work/morning-check.md`: your check of every amount and every reminder, and what you corrected
- `work/chatgpt-review.md`: ChatGPT's second opinion on a sample of the pack
- `NOTES.md`: your answer to the case's final assessment, and the discussion questions

## Key concepts

- **Statement:** a list of a customer's open invoices, payments and credits, with the balance (policy, Appendix B).
- **Statement pack:** one statement, and a draft reminder where due, for each customer with an overdue invoice.
- **Standing instructions:** the project's written instructions, read at the start of every run.
- **Memory:** what an app remembers from earlier chats. It is not a reliable place for rules a run must follow.
- **Release:** the moment a person decides a piece of work may go out. In this bootcamp, nothing is ever actually sent.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync and start a thread.** Sync your fork, pull in GitHub Desktop, and start a new thread for this step.

**2. Write the brief once.** Paste:

```text
I'm doing Step 05 of the bootcamp. Help me write step-05-overnight-client-job/work/brief.md, the brief for an overnight job. Don't run the job yet.

Outcome: for every Copperleaf customer with an invoice past its due date on Monday 2 November 2026, a statement of the account and, where copperleaf/policies/credit-and-collections-policy.md section 5.1 calls for one, a draft reminder for the highest stage reached, so Rosa can check and sign them in the morning.

Context: open invoices and days overdue are in step-02-three-deliverables/work/claude/figures.csv. Customer names and contacts are in copperleaf/customers.csv. Use the policy for the schedule, and say which stage and section each reminder follows. Leave disputed invoices out of reminders (6.2), but show them on the statement marked "in dispute". The 45-day final notice is signed by the Finance Manager (5.1, 11). A hold at 60 days is proposed by the Credit Controller and approved by the Finance Manager (4.3).

Format: one Markdown file per customer in step-05-overnight-client-job/work/statement-pack/, named <customer_id>-<short-name>.md, with the statement first and the draft reminder (if any) below it, marked "DRAFT, NOT SENT". Plus step-05-overnight-client-job/work/statement-pack/index.md, a table of every customer in the pack, the balance, the stage and the file name.

Constraints: draft only; send nothing and contact nobody. Use only those files. Leave out contact names (policy 10.2): address each letter to the customer's accounts team. If something doesn't fit the policy, write it in index.md under "Needs a person" instead of guessing. Never commit or push.

Show me the brief before you save it.
```

Read it and correct anything that's unclear. Someone who has never seen this thread must be able to do the job from the brief alone.

**3. Lock what matters, and test the lock.** Make sure your project instructions still say never to send, and that the thread asks before it acts (step 3). Then test it in this thread:

```text
Test: while doing the overnight job, could you send the reminders, or change any file in the copperleaf folder? Don't try; tell me what would stop you, and what you'd do if the brief seemed to ask for it.
```

If the answer is anything other than "I would stop and ask", fix your instructions first.

**4. Ask for the overnight run.** Schedule a task in this project for tonight (or start it in a new thread before you stop for the day, with your computer awake), with this instruction. If your computer will be off overnight, run it as a cloud session on your fork instead and review its branch in the morning. [Finding things in the apps](../step-00-readiness-check/README.md#a-scheduled-task) and the section after it show both, click by click:

```text
Do the job in step-05-overnight-client-job/work/brief.md exactly as written. Read the brief first; you don't know anything else about it. When you finish, add to the end of work/statement-pack/index.md: the time you finished, the files you read, and anything you weren't sure of.
```

Keep your computer awake if it runs on your computer.

**5. The morning check.** Open `work/statement-pack/index.md` first, then do every check in [Check it](#check-it). Record each finding, and what you corrected, in `work/morning-check.md`. Ask Claude to fix a letter only by naming the letter and the exact problem.

**6. Instructions or memory?** Paste in a fresh thread:

```text
Without reading any file: what is Copperleaf's reminder schedule? Then tell me where your answer came from.
```

In `NOTES.md`, write what this shows about relying on memory for a nightly run.

## Repeat it in ChatGPT

In this step, ChatGPT gives the **second opinion** on a sample, as in the case.

1. Pick three letters from the pack: the longest, one with a 21-day reminder, and one you think may be wrong.
2. In your ChatGPT project (or, without one, a new chat with the same files attached), attach those three files, `figures.csv`, `customers.csv` and the policy, and paste:

```text
You are reviewing three draft letters from an overnight job before a person signs them. For each, check every amount against figures.csv, the reminder stage against the policy's section 5.1 and the rules in sections 5.2, 6.2 and 10.2. List each problem with the line it's on. Don't rewrite the letters.
```

3. Save the answer as `work/chatgpt-review.md`, and mark each point *accepted* or *rejected* with a reason.

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **The right customers.** Every customer with an invoice past its due date in `figures.csv` has a statement, and no one else does. Count them yourself.
- [ ] **Every amount.** For each statement, the invoices and the balance match `figures.csv`. Add up two balances yourself.
- [ ] **Every stage.** For each reminder, work out the days overdue of the oldest invoice and check the stage against section 5.1. No reminder for an invoice under 7 days overdue.
- [ ] **The disputed invoice** is marked "in dispute" on its statement and has no reminder.
- [ ] **Who signs.** The final notice says the Finance Manager signs. Any hold is a proposal for the Finance Manager to approve, and says the Owner is told where the limit is above 10,000.
- [ ] **No personal details.** No contact names; no bank details.
- [ ] **"Needs a person" was used.** Anything the run wasn't sure of is listed, not guessed.
- [ ] **Nothing sent, nothing else changed.** GitHub Desktop shows changes only in this step's folder.

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-05: overnight statement pack` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-05-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/brief.md`
- [ ] `work/statement-pack/` with `index.md` and one file per customer
- [ ] `work/morning-check.md`, with every check above and what you corrected
- [ ] `work/chatgpt-review.md` (or a transfer plan in `NOTES.md`)
- [ ] **Checked:** every amount and every reminder stage checked by you against the ledger figures and policy 5.1
- [ ] `NOTES.md`: your answer to the [final assessment](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-2-nishas-first-client/final-assessment-a-new-ai-worker/), the discussion questions, and what step 6 showed about memory
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] Committed, tagged `step-05-done` and pushed

## References

- [Case 2: Nisha's First Client](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-2-nishas-first-client/overview/)
- [Work that runs while you sleep](https://agentfactory.panaversity.org/claude-and-chatgpt-2/behind-the-screen/work-that-runs-while-you-sleep/)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md), sections 4, 5, 6, 10 and 11

---

[← Step 04: A Second Opinion and the Human Check](../step-04-second-opinion/) · [Roadmap](../README.md#roadmap) · [Step 06: A Worker the Whole Team Shares →](../step-06-shared-worker/)
