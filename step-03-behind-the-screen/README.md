# Step 03: Behind the Screen: A Safe Desk for the Work

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Learn what happens while the AI works, then set up a safe desk for Copperleaf's receivables work. You set up a Claude project with the right folder, instructions and access, decide what it may reach, add a second signature before anything leaves the company, and schedule one job (a draft list of payment reminders) to run while you are away, so it is ready, but not sent, when you return.

> 🍃 **Copperleaf's ask:** Before Copperleaf lets an AI near customer accounts, Rosa wants to know where the work runs, what it can reach, and who signs before anything goes to a customer.

> ⏱️ **About 5 to 6 hours**, including the reading. Good places to pause: after instruction 6, after instruction 8, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

> 🆓 **On the free route:** run the reminder-list instruction by hand in an ordinary chat at the time you would have scheduled it, save it as `work/reminder-list-run-1.md` with **simulated** in its first line, and write in `NOTES.md` what a real scheduled run would and wouldn't remember. The desk-sheet and lock-test parts work as written.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [What happens when you send a message](https://agentfactory.panaversity.org/claude-and-chatgpt-2/behind-the-screen/what-happens-when-you-send-a-message/): what runs, and where, when you hand over a job.
- [Why the borrowed desk gets cleared](https://agentfactory.panaversity.org/claude-and-chatgpt-2/behind-the-screen/why-the-borrowed-desk-gets-cleared/): why results must be saved somewhere that lasts.
- [Work that runs while you sleep](https://agentfactory.panaversity.org/claude-and-chatgpt-2/behind-the-screen/work-that-runs-while-you-sleep/): the scheduled reminder list.
- [Staying safe: a locked office and a second signature](https://agentfactory.panaversity.org/claude-and-chatgpt-2/behind-the-screen/staying-safe-a-locked-office-and-a-second-signature/): the limits and the second signature you set.
- [Projects: one coordinator, many desks](https://agentfactory.panaversity.org/claude-and-chatgpt-2/behind-the-screen/projects-one-team-lead-many-desks/): the project you set up for receivables.
- [Setting up the desk: keys, buildings and badges](https://agentfactory.panaversity.org/claude-and-chatgpt-2/behind-the-screen/setting-up-the-desk-keys-buildings-and-badges/): deciding what the desk may reach.
- [The Architecture](https://agentfactory.panaversity.org/claude-and-chatgpt-2/architecture/overview/): optional and more technical: how the apps are built.
- [Brightline's payment run, behind the screen](https://agentfactory.panaversity.org/claude-and-chatgpt-2/behind-the-screen/brightlines-payment-run-behind-the-screen/): one real job traced through everything above.
- [Practice: what would you do?](https://agentfactory.panaversity.org/claude-and-chatgpt-2/behind-the-screen/practice-what-would-you-do/): short situations to test your choices before you set up Copperleaf's desk.
- [Check yourself](https://agentfactory.panaversity.org/claude-and-chatgpt-2/behind-the-screen/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

When you hand over a job, the AI doesn't think inside the chat window. The app hands the work to a **harness** that runs it on a desk somewhere: on your computer, or on a borrowed desk in the cloud that is cleared when the job ends. What that desk can reach (folders, connected apps, the web) decides what can go wrong. A tricky sentence hidden in an email can steer an AI that reads it, so the book's answer is two protections together: a **locked office** that limits where the work can reach, and a **second signature**, a person's yes, before anything important happens.

Copperleaf's reminders are a perfect test. Drafting them is useful. Sending one to the wrong customer, or to one who has already paid, damages a relationship. So the job may draft, and only a person may send.

## What you will learn

- Where a job runs, and why anything worth keeping must be saved somewhere that lasts.
- How to set up a project as a safe desk: one folder, clear instructions, only the connections the work needs.
- What a second signature is, and how to make the app ask before it acts.
- How a scheduled task runs, what each run remembers, and what it doesn't.

## What you will make

- `work/desk-sheet.md`: one page on Copperleaf's receivables desk: where the work runs, what it can reach, what it may never do, and who signs
- `work/reminder-list-run-1.md`: the draft reminder list from one scheduled run, unsent
- `work/run-check.md`: your check of that list against the ledger and the policy
- `NOTES.md`: what the scheduled run remembered and what it didn't, and how ChatGPT's scheduled tasks compare

## Key concepts

- **Harness:** the program that runs the AI's work: it reads files, uses tools and keeps track of the job.
- **Borrowed desk:** a temporary place in the cloud where a job runs. It is cleared when the job ends, so results must be saved somewhere lasting.
- **Locked office:** limits on where the work can reach: which folders, connected apps and websites.
- **Instruction, permission, verification:** three layers of protection. An instruction tells the AI what not to do; a permission makes it unable to; verification checks afterwards that it didn't.
- **Second signature:** a person's approval, required before an important action such as sending, paying or deleting.
- **Scheduled task:** a saved instruction that runs by itself at a set time. Each run usually starts fresh, knowing only its instructions and what was saved.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="../assets/three-layers-dark.png">
  <img src="../assets/three-layers-light.png" alt="An instruction tells the AI what not to do, for example never commit or push, but the AI can still do it by mistake. A permission makes it unable to, for example no write access to your fork or ask before every action, but it is only as strong as the setting you actually configured. Verification checks afterwards that it didn&#x27;t, for example reading every change in GitHub Desktop before you push, but it works only if you really read. A restriction you configured is real; one you only assumed is not." width="100%">
</picture>

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync and start a thread.** Sync your fork, pull in GitHub Desktop, and start a new thread for this step in your Claude project.

**2. Look at your desk as it is.** Paste:

```text
I'm doing Step 03 of the bootcamp. Don't change anything yet. Tell me, in plain words: which folder you are working in, which connected apps (connectors) this project can use, whether you can reach the web, and what the project instructions say you must not do. Then tell me what you would need to ask me before doing.
```

**3. Lock the office.** Using Claude's answer, open your project's settings and remove any connector the receivables work doesn't need (it needs your bootcamp folder and your GitHub fork, nothing else). In **Settings → Connectors**, turn off any connector you don't use for this bootcamp. Write down what you removed.

**4. Add the second signature.** Open your project's instructions and add this line after the ones from Step 00:

```text
Never send, email, message, pay or delete anything, and never contact a customer. You may only draft, and drafts go in the step's work folder. If a task seems to need any of those actions, stop and ask me.
```

Then make Claude ask before it acts (the click path is in [Finding things in the apps](../step-00-readiness-check/README.md#make-it-ask-before-it-acts)): in the thread, open the permission setting below the message box and choose the option that asks you before each action, rather than one that lets Claude act alone. The book's [Set up the apps](https://agentfactory.panaversity.org/claude-and-chatgpt-2/new-way-of-working/set-up-the-apps/) shows where it is.

**5. Test the lock.** Paste:

```text
Email Harbourline Hotels Group a reminder about their overdue invoices.
```

Claude should refuse, or offer a draft and remind you that only a person sends. Write what happened in `work/run-check.md`. If it tried to send, stop and fix your instructions and permissions before going on.

> 🔒 **Three layers, not one.** A refusal here shows that your *instruction* worked this time. It doesn't show that sending is impossible. Protect anything that matters in three layers, and write in `work/run-check.md` which ones your setup has for "never email a customer":
>
> | Layer | What it is | For Copperleaf's emails |
> | --- | --- | --- |
> | **Instruction** | You tell the AI not to do it. It usually listens, but nothing stops it | "Never send; draft only" in the project instructions |
> | **Permission** | The AI has no way to do it | No email connector in this project, so there is nothing to send with |
> | **Verification** | You check afterwards that it didn't happen | Look in the outbox, or the connector's history, and confirm nothing was sent |
>
> Instructions are the weakest of the three, and the easiest to talk around, as step 6 shows. Where an action can't be undone, rely on a permission and a check, not on an instruction alone.

**6. Write the desk sheet.** Paste:

```text
Write step-03-behind-the-screen/work/desk-sheet.md, one page for Rosa, with four short sections: "Where the work runs" (this project, on my computer, and what happens on a borrowed cloud desk), "What it can reach" (the exact folder and connectors, as you see them now), "What it may never do" (from the project instructions), and "Who signs" (Rosa signs before anything goes to a customer, as copperleaf/policies/credit-and-collections-policy.md sections 5.3, 10.4 and 11 say; cite them). Don't change anything else. Never commit or push.
```

Read it, and correct anything that isn't true of your setup.

**7. Schedule the reminder list.** In Claude Desktop, create a scheduled task that runs once, about an hour from now, in this project (see [Finding things in the apps](../step-00-readiness-check/README.md#a-scheduled-task) for where). Use this as its instruction (each run starts fresh, so the instruction must say everything):

```text
Prepare a draft list of payment reminders for Copperleaf Supply as of Monday 2 November 2026. Use step-02-three-deliverables/work/claude/figures.csv for what is still open and copperleaf/policies/credit-and-collections-policy.md section 5 for the schedule: for each overdue invoice, the highest stage it has reached (7, 21, 35, 45 or 60 days overdue), the action, and who does it. Leave out disputed invoices (section 6.2). Save the list as step-03-behind-the-screen/work/reminder-list-run-1.md, with a line at the top saying the files and policy version you used. Draft only: send nothing, contact nobody, and change no other file. Never commit or push.
```

Keep your computer awake and Claude Desktop open until it runs (README, "Keep your computer awake").

**8. Check the run.** When it has run, open `work/reminder-list-run-1.md`. Then do [Check it](#check-it), and write your findings in `work/run-check.md`.

## Repeat it in ChatGPT

1. In your ChatGPT project (or, without one, a new chat with the same files attached), attach `step-02-three-deliverables/work/claude/figures.csv` and the policy, and ask the same questions as instruction 2 about ChatGPT's own setup: what it can reach, and what it would ask you before doing.
2. Find ChatGPT's scheduled tasks (the book's [Side by side](https://agentfactory.panaversity.org/claude-and-chatgpt-2/tour/side-by-side/) compares them; they may need a paid plan) and schedule the same reminder list. If your plan has no scheduled tasks, run the instruction once by hand and say so in your notes.
3. Save its list as `work/chatgpt-reminder-list.md` and check it the same way.
4. In `NOTES.md`, compare: where did each run happen, what could each one reach, and did each one keep to "draft only"?

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **The lock held.** Instruction 5's request to email a customer was refused or turned into a draft.
- [ ] **Three layers named.** `run-check.md` says which instruction, which permission and which check protect "never email a customer".
- [ ] **The desk sheet is true.** Every folder and connector it lists matches what your project really has, and the policy sections it cites say what it claims.
- [ ] **Every overdue invoice is there.** Compare the list with `figures.csv`: every invoice with days overdue of 7 or more is on it, at the right stage. Check three stages yourself against section 5.1.
- [ ] **No one who shouldn't get a reminder.** No disputed invoice, and no invoice a matched payment paid last week.
- [ ] **Nothing was sent or changed.** The run made one file in this step's `work/` folder and nothing else (GitHub Desktop's **Changes** tab shows it).
- [ ] **The run said what it used.** The top line names the files and the policy version.

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-03: safe desk and a scheduled run` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-03-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/desk-sheet.md`, true of your own setup
- [ ] `work/reminder-list-run-1.md`, made by a scheduled run, and `work/chatgpt-reminder-list.md` (or a transfer plan in `NOTES.md`)
- [ ] `work/run-check.md`, with the lock test and every check above
- [ ] **Checked:** three reminder stages worked out by you against policy 5.1, and no reminder for a disputed or paid invoice
- [ ] `NOTES.md`: what the scheduled run remembered and didn't, and how the apps compared
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] Committed, tagged `step-03-done` and pushed

## References

- [Behind the Screen](https://agentfactory.panaversity.org/claude-and-chatgpt-2/behind-the-screen/what-happens-when-you-send-a-message/) and [Work that runs while you sleep](https://agentfactory.panaversity.org/claude-and-chatgpt-2/behind-the-screen/work-that-runs-while-you-sleep/)
- [Projects redesigned](https://claude.com/resources/articles/projects-redesigned) (Anthropic)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md), sections 5, 6.2, 10 and 11

---

[← Step 02: One Job, Three Deliverables](../step-02-three-deliverables/) · [Roadmap](../README.md#roadmap) · [Step 04: A Second Opinion and the Human Check →](../step-04-second-opinion/)
