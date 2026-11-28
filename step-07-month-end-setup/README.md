# Step 07: One Setup for the Month-End

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Follow the book's fourth case. Copperleaf's month-end receivables report takes two days of copying between files. You join the features you already use (a project, a skill, and a small script that Claude writes and you check by its results, not by reading it) into one setup, run it for October, and check the report before Rosa sees it. This step ends the first milestone.

> 🍃 **Copperleaf's ask:** Rosa wants the month-end receivables report ready on the first working morning of each month, built the same way every time, whoever runs it.

> ⏱️ **About 6 to 8 hours**, including the reading. Good places to pause: after instruction 4, after instruction 6, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

> 🆓 **On the free route:** paste the skill's steps into an ordinary chat instead of adding the skill, and mark it **simulated**. The script, the run and the tests work as written.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [Case 4: Nisha's Month-End](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-4-nishas-month-end/overview/): the case this step follows.
- [Two days of copying](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-4-nishas-month-end/two-days-of-copying/): the problem the setup solves.
- [One place for Northgate](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-4-nishas-month-end/one-place-for-lakeshore/): keeping a client's files in one place.
- [The run](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-4-nishas-month-end/the-run/): what the month-end run does, step by step.
- [Lab: build the month-end](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-4-nishas-month-end/lab-build-the-month-end/): the book's version of the setup. The Copperleaf job below replaces it.
- [What the setup did](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-4-nishas-month-end/what-the-setup-did/): what each part of the setup was for.
- [Final assessment: four questions](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-4-nishas-month-end/final-assessment-four-questions/): the final assessment for the whole first section.
- [Exhibits](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-4-nishas-month-end/exhibits/): the case's documents.
- [Questions for discussion](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-4-nishas-month-end/questions-for-discussion/): the questions you answer in your notes.
- [Check yourself](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-4-nishas-month-end/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

In steps 1 to 6 you used each feature on its own: a brief, deliverables, a project, a scheduled run, a second opinion, a skill. Month-end work is where they come together. A report that is rebuilt by hand each month comes out slightly different each time, depending on who builds it. A **setup** fixes that: the project holds the files and the standing instructions, the skill holds the steps, and a small script does the arithmetic the same way every time. Then any of the team can run it and get the same report.

You don't need to read code. You check a script the way an accountant checks a calculator: give it inputs whose answer you already know, and see if it gets that answer.

## What you will learn

- How a project, a skill and a script divide one recurring job between them.
- How to check a script by its results, using figures you have already checked.
- How to fix a mistake by hand, then make the next run pick it up.
- What each part of a setup is for, and what still needs a person.

## What you will make

- `work/month-end/instructions.md`: the standing instructions for the month-end job
- `work/month-end/skill/copperleaf-month-end/SKILL.md`: the skill with the job's steps
- `work/month-end/build_report.py`: the script Claude writes, which you check by its results
- `work/month-end/corrections.csv`: corrections a person has confirmed, read by every run
- `work/month-end/october-report.md`: October's report, from the first run and again after a correction
- `work/test-and-approval.md`: how you tested the setup, and Rosa's approval
- `NOTES.md`: your answers to the four final-assessment questions and the discussion questions
- A recorded project defence, because this step ends milestone 1

## Key concepts

- **Setup:** the project, instructions, skill and script that together do a recurring job the same way each time.
- **Script:** a short program that does the arithmetic. Claude writes it; you check it by its results.
- **Check by results:** run the script on inputs whose answer you already know, and compare.
- **Corrections file:** a file of fixes a person has confirmed, which every run applies, so a fix made by hand isn't lost next month.
- **Month-end report:** the summary of what customers owe at the end of a month: totals by age band, overdue accounts, holds, disputes and unmatched money.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync and start a thread.** Sync your fork, pull in GitHub Desktop, and start a new thread for this step.

**2. Make the two files the job needs.** Paste:

```text
I'm doing Step 07 of the bootcamp. Make two files, and nothing else yet:

1. step-07-month-end-setup/work/month-end/instructions.md: standing instructions for Copperleaf's month-end receivables report. Inputs: copperleaf/invoices.csv, copperleaf/payments-week-44.csv, copperleaf/customers.csv, the policy, and work/month-end/corrections.csv. Rules: apply a payment only when payer, reference and amount match one open invoice exactly, or when corrections.csv confirms it (policy 8.1); hold everything else as unallocated; age every open invoice as of the run date; keep disputed invoices out of the bands; draft only, send nothing; say at the top which files and policy version were used.
2. step-07-month-end-setup/work/month-end/corrections.csv, with the columns payment_id, invoice_no, confirmed_by, date and note, and no rows yet.

Show me both before saving. Never commit or push.
```

**3. Build the setup.** Paste:

```text
Now write two more files:

1. step-07-month-end-setup/work/month-end/build_report.py, a short Python script that follows instructions.md exactly and writes step-07-month-end-setup/work/month-end/october-report.md with: run date and inputs; total open; totals by band (not yet due, 1-30, 31-60, 61-90, over 90); disputed total; unallocated payments with their total; the five largest balances against their credit limits; accounts that meet the hold rule in policy 4.1; and invoices at the 45-day final-notice stage. Add short comments that say why, not what.
2. step-07-month-end-setup/work/month-end/skill/copperleaf-month-end/SKILL.md: the steps to run it: read instructions.md, run the script with the run date, check the report's totals add up, list anything unallocated or needing a person, and stop; never send.

Explain in five plain sentences what the script does. Then wait.
```

**4. Run it for October.** Paste:

```text
Run build_report.py with the run date 2026-11-02, the first working morning of November. Show me the report, and don't change any other file.
```

> 💡 **The script needs Python, and you don't have to install it yourself first.** Python is a programming language, and `build_report.py` is a short program in it. Claude writes it and runs it for you. Often it runs on Claude's own computer in the cloud, which already has Python. If it runs on your computer and Claude says Python isn't installed: on a Mac, a window may offer to install the "command line developer tools"; click **Install**, wait for it to finish, and ask Claude to try again. On Windows, install Python from [python.org](https://www.python.org/downloads/) (on the first screen, tick **Add python.exe to PATH**), restart Claude Desktop, and ask again. If you would rather install nothing, ask: `Run build_report.py on your own computer in the cloud, not mine, and save the report into my folder.` You never need to read or edit the code; you test it by its results, below.

**5. Test it by its results.** You already checked these figures in step 2. Compare the report with your checked `step-02-three-deliverables/work/claude/figures.csv` and `work/my-checks.md`: the total open, each band total and the disputed total must agree. If they don't, find out which one is right before going on, and write it all in `work/test-and-approval.md`. Then test one thing you know the answer to that step 2 didn't cover: does the hold list match what section 4.1 says for every account over 60 days overdue?

**6. Fix it by hand, then run again.** Riverside Deli's payment with the reference "OCT STATEMENT" was unallocated. Pretend Ben has now phoned Riverside, and they confirmed it pays INV-4220. Add one row to `work/month-end/corrections.csv` by asking Claude:

```text
Add a row to corrections.csv: PAY-9037 pays INV-4220, confirmed by Ben by phone on 2 November 2026. Change nothing else.
```

Run the script again. Check that only what should change did: INV-4220 is no longer open, the 1 to 30 days band and the total open each fall by that amount, and the unallocated total falls by the same amount.

**7. Add the skill to the project.** Zip the `skill/copperleaf-month-end` folder and add it in **Customize → Skills**, as in step 6. In a fresh thread, ask `Run the Copperleaf month-end report for the run date 2026-11-02.` and check you get the same report.

**8. Approve it.** Add Rosa's approval to `work/test-and-approval.md`, naming the files it covers (instructions, skill, script and corrections file) and the date.

## Repeat it in ChatGPT

1. In your ChatGPT project (or, without one, a new chat with the same files attached), attach the five input files, `instructions.md` and `build_report.py`.
2. Ask ChatGPT to run the script with the run date 2026-11-02 (it runs code in its own environment) and give you the report to download. Save it as `work/chatgpt-october-report.md`.
3. Compare it with Claude's report: every figure must match, because the script and the inputs are the same. If anything differs, find out why.

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

> 🌍 **Optional: in your own field.** Think of one task you repeat every month in your own work. Write its standing instructions (inputs, rules, what it never does) in `NOTES.md`, as you did for the month-end report, and say how you would test the setup by its results. Describe it with made-up examples, never real data. See the README's [examples by profession](../README.md#your-client-copperleaf-supply).

## Check it

- [ ] **The report matches your checked figures.** Total open, every band and the disputed total agree with step 2.
- [ ] **The hold list is right.** Every account it lists meets section 4.1, and every account that meets 4.1 is on it.
- [ ] **The correction worked, and only it.** After the second run, the changes are exactly the ones in instruction 6.
- [ ] **The run says what it used.** Inputs, run date and policy version are at the top of the report.
- [ ] **Same result, fresh thread.** The skill gives the same report in a new thread.
- [ ] **Nothing else changed.** No file outside this step's folder.

## Record your defence

This step ends milestone 1, so record a project defence of up to five minutes ([SUBMITTING.md, section 10](../SUBMITTING.md#10-defend-your-work)). Show the setup running; trace one figure in the report back to the invoices; explain one thing the setup may never do and how you made sure; and show one change you made to what Claude produced.

Before you share it, go through the [privacy checklist](../SUBMITTING.md#before-you-share-a-screenshot-or-recording).

## Keep it

Do this last, after the ChatGPT part, your notes and your defence. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-07: month-end setup and October report` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-07-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/month-end/` with `instructions.md`, `corrections.csv`, `build_report.py`, the skill and `october-report.md`
- [ ] `work/test-and-approval.md`, with the test by results, the correction rerun and Rosa's approval
- [ ] `work/chatgpt-october-report.md` (or a transfer plan in `NOTES.md`)
- [ ] **Checked:** the report's totals compared with your checked step 2 figures, and the hold list checked against policy 4.1
- [ ] `NOTES.md`: your answers to the [four questions](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-4-nishas-month-end/final-assessment-four-questions/) and the discussion questions
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] **Defence:** a link to your recorded project defence, ready for the form
- [ ] Committed, tagged `step-07-done` and pushed

## References

- [Case 4: Nisha's Month-End](https://agentfactory.panaversity.org/claude-and-chatgpt-2/case-4-nishas-month-end/overview/)
- [Use skills in Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude) (Anthropic)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md), sections 4 and 8

---

[← Step 06: A Worker the Whole Team Shares](../step-06-shared-worker/) · [Roadmap](../README.md#roadmap) · [Step 08: The Big Picture: From Chatbot to AI Worker →](../step-08-the-big-picture/)
