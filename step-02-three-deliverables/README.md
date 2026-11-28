# Step 02: One Job, Three Deliverables

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Turn one piece of receivables work into the three things a business actually uses: a spreadsheet, a document and a short deck. From Copperleaf's open invoices you make an aged receivables sheet, a one-page memo on the accounts most overdue, and five slides for the owner's Monday meeting, and you save each one where the team can find it.

> 🍃 **Copperleaf's ask:** Amira, Copperleaf's owner, asks every month how much customers owe and who is late. She wants one sheet she can sort, one page she can read, and slides she can show the bank.

> ⏱️ **About 6 to 8 hours**, including the reading. Good places to pause: after instruction 4, after instruction 6a, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [Build Something](https://agentfactory.panaversity.org/claude-and-chatgpt-2/build-something/overview/): what the apps can make, and in what form.
- [Where your work is saved](https://agentfactory.panaversity.org/claude-and-chatgpt-2/build-something/where-your-work-is-saved/): where each deliverable ends up, and how to keep it.
- [Sheets](https://agentfactory.panaversity.org/claude-and-chatgpt-2/build-something/sheets/): the aged receivables sheet.
- [Docs](https://agentfactory.panaversity.org/claude-and-chatgpt-2/build-something/docs/): the one-page memo.
- [Slides](https://agentfactory.panaversity.org/claude-and-chatgpt-2/build-something/slides/): the five slides.
- [One job, three deliverables](https://agentfactory.panaversity.org/claude-and-chatgpt-2/build-something/one-job-three-deliverables/): the pattern this step follows, and the book's version of this step.
- [Data](https://agentfactory.panaversity.org/claude-and-chatgpt-2/build-something/data/): working with a table of data, and, under "Going further", a dashboard connected to practice data (paid plan): the book's place to connect a data source.
- [Design](https://agentfactory.panaversity.org/claude-and-chatgpt-2/build-something/design/) and [Whiteboard](https://agentfactory.panaversity.org/claude-and-chatgpt-2/build-something/whiteboard/): optional: two more forms a deliverable can take.
- [Check yourself](https://agentfactory.panaversity.org/claude-and-chatgpt-2/build-something/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

In step 1 the AI gave you a table and a page of text. Real work arrives in other shapes: a spreadsheet someone sorts and filters, a document someone signs, slides someone presents. The apps can now make all three as real files. The skill is not "make slides". It is keeping one set of facts true in every shape: if the sheet says customers owe one amount and the slides say another, the bank stops trusting all of it.

An **aged receivables report** sorts what customers owe by how late it is. It is one of the first things an owner, an auditor or a bank asks for, so it is worth getting exactly right.

## What you will learn

- How to ask for a deliverable in the form its reader needs: a sheet, a document or a deck.
- How to make three deliverables from one set of figures, so they agree.
- Where each app saves what it makes, and how to keep it in your folder.
- How to check a deliverable's numbers against its sources, not against each other.
- Optional, on a paid plan: when a connector to your data beats uploading a file.

## What you will make

All in this step's `work/` folder:

- `work/claude/aged-receivables.xlsx`: every open invoice with its customer, due date, days overdue and age band, and a summary of totals by band and by customer
- `work/claude/overdue-memo.docx`: a one-page memo to Amira on the accounts most overdue, with what the policy says to do about each
- `work/claude/monday-slides.pptx`: five slides for Amira's Monday meeting
- `work/claude/figures.csv`: the checked figures every later step uses
- `work/chatgpt/`: the same four files made in ChatGPT
- `work/my-checks.md`: the three totals you worked out by hand, and whether all three deliverables agree
- Optional, on a paid plan: `work/dashboard-note.md`, on the same view built as a dashboard through a connector
- `work/memo-rounds.md`: the memo's review rounds with the Dr. Gilsdorf method, each with its grade, and the second AI's review
- `NOTES.md`: what each app did well, and where each one saved its files

## Key concepts

- **Aged receivables:** what customers owe, sorted into age bands by how many days each invoice is past its due date.
- **Age band:** a range of days overdue, here: not yet due, 1 to 30 days, 31 to 60, 61 to 90 and over 90.
- **Days overdue:** the number of days from an invoice's due date to the report date. Copperleaf's report date is Monday 2 November 2026.
- **Deliverable:** a finished piece of work in the form its reader uses, such as a sheet, a document or a deck.
- **The Dr. Gilsdorf method:** improving a piece of work in many small rounds, by asking the best available AI to review and grade it out of 10 each time, and finishing with an independent review from a different AI.
- **Connector:** a link that lets the app read from another service, such as Google Drive, instead of a file you upload.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync and start a thread.** Sync your fork and pull in GitHub Desktop, as in step 1. Then start a new thread for this step in your Claude project.

**2. Check that Claude can make files.** In Claude Desktop, **Settings → Capabilities** must have file creation turned on (Step 00, A6). Without it, Claude can describe a spreadsheet but can't make one.

**3. Settle the figures first.** One set of figures, then three shapes. Paste:

```text
I'm doing Step 02 of the bootcamp. First, settle the figures, and make no deliverables yet.

Start from copperleaf/invoices.csv (the ledger before last week's payments) and apply last week's payments using my checked matches in step-01-first-whole-job/work/claude/payment-matches.csv: apply only rows marked "matched", and anything I noted in step-01-first-whole-job/work/my-checks.md. Leave every "needs a person" payment unapplied.

Then, as of Monday 2 November 2026, list every invoice still open, with customer, invoice date, due date, amount still open, days overdue (2 November minus the due date) and age band: not yet due, 1-30, 31-60, 61-90, over 90. Keep disputed invoices out of the bands and show them on their own line.

Save it as step-02-three-deliverables/work/claude/figures.csv and tell me: the total still open, the total in each band, the disputed total, and the five customers who owe most. Don't change anything in the copperleaf folder. Never commit or push.
```

**4. Check the figures before anything else.** Do the first three checks in [Check it](#check-it) now. A mistake here would be copied into all three deliverables.

**5. Make the sheet.** Paste:

```text
Using only step-02-three-deliverables/work/claude/figures.csv, make an Excel workbook, step-02-three-deliverables/work/claude/aged-receivables.xlsx, with two sheets:
1. "Invoices": every row, with a filter on the header row, sorted by days overdue, oldest first.
2. "Summary": the total in each age band and the disputed total, using formulas that add up the Invoices sheet (not typed numbers), then one row per customer with its total and its oldest days overdue.
Tell me which cells hold the grand total.
```

**6. Make the memo.** Paste:

```text
Using the same figures and copperleaf/policies/credit-and-collections-policy.md, write a one-page Word memo to Amira, step-02-three-deliverables/work/claude/overdue-memo.docx. Cover: the total owed, how much is overdue, and the accounts with any invoice more than 30 days overdue. For each of those accounts, say what the policy's reminder schedule (section 5) and hold rule (section 4) call for now, citing the section. Recommend nothing the policy doesn't support, and mark anything that needs Rosa's or Amira's decision.
```

**6a. Improve the memo: the Dr. Gilsdorf method (about 45 minutes).** Good writing is rewritten, many times, in small steps. Zia Khan, who leads this bootcamp, learned this from Dr. Gilsdorf, a business communication professor at Arizona State University, and calls this way of working with AI the **Dr. Gilsdorf method**: ask the best model you have to review and grade your work out of 10, improve it a little, and repeat; then, as a last step, give it to a *different* AI for an independent review and bring that review back. Iteration is the key. The book describes it in [How the Panaversity team works, "How do we improve the work?"](https://agentfactory.panaversity.org/claude-and-chatgpt-2/new-way-of-working/how-the-panaversity-team-works/#how-do-we-improve-the-work). Try it on the memo:

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="../assets/gilsdorf-method-dark.png">
  <img src="../assets/gilsdorf-method-light.png" alt="Start with your draft. Ask the best AI you have to run the checks, such as every figure matching its source, and grade the work out of 10. Improve it in one small step, then check and grade again, and repeat until every check passes and the grade reaches 9.5. Then give the work to a different AI for an independent review, without the first AI's grades, paste that review back into your first AI, fix what is right and run the checks again. You check the facts and read every change before you commit it. A failed check always outweighs a grade." width="100%">
</picture>

1. **Round 1: review and grade.** Paste:

   ```text
   Review step-02-three-deliverables/work/claude/overdue-memo.docx as Amira, Copperleaf's owner, would read it. Grade it out of 10, and list the three changes that would raise the grade most, in order. Don't change the memo yet. Save the grade and the list as "Round 1" in step-02-three-deliverables/work/memo-rounds.md.
   ```

2. **Improve in a small step.** Read the list, decide which changes you agree with, and ask for only those: `Make changes 1 and 2 from Round 1, and nothing else. Keep every figure exactly as it is in figures.csv.`
3. **Rounds 2 and 3.** Ask for the review and grade again (`Same review, as "Round 2"`), and improve again. Stop when the grade stops rising, or after three rounds.
4. **A second AI's review.** In ChatGPT, attach the memo and `figures.csv`, and paste:

   ```text
   Review this memo for Copperleaf's owner. Grade it out of 10 and list what would most improve it. Say if any figure doesn't match figures.csv.
   ```

   Copy ChatGPT's answer into `memo-rounds.md` as "Second AI", then paste it back into your Claude thread: `Here is an independent review from another AI. Which points do you agree with, and which not? Make only the ones I approve:` followed by the points you approve.
5. **Record it.** In `memo-rounds.md`, keep the grade from each round in a short table.

> ⚠️ **A grade is an opinion, not a check.** An AI can give a 9 to a memo with a wrong number in it, and two AIs can disagree. The method makes writing clearer; it doesn't make facts true. You still check every figure yourself (instruction 9). And only share work with another AI company when you are allowed to: Copperleaf's files are made up, but at your own job, confidential content stays with the tools your organization has approved.

**7. Make the slides.** Paste:

```text
Using the same figures, make five slides for Amira's Monday meeting, step-02-three-deliverables/work/claude/monday-slides.pptx: 1) title and report date, 2) total owed and how much is overdue, 3) a bar chart of the age bands, 4) the five largest balances, 5) what needs a decision this week. Every number must come from figures.csv. Put the source file and date in a small footer on slides 2 to 5.
```

**8. Open all three.** Open each file from your folder in its app (Excel, Numbers or Google Sheets for the sheet; Word or Pages for the memo; PowerPoint or Keynote for the slides). If a file won't open, tell Claude which one and what you saw.

**9. Check them.** Do the rest of [Check it](#check-it), and write your results in `work/my-checks.md`.

**10. Optional, on a paid plan: a connector.** Copy the `copperleaf` folder's CSV files into a folder in your own Google Drive. In Claude, connect Google Drive (**Settings → Connectors**), and ask for the same summary as a dashboard that reads from that Drive folder, following the book's [Data, "Going further"](https://agentfactory.panaversity.org/claude-and-chatgpt-2/build-something/data/). In `work/dashboard-note.md`, write when a connector beats an upload (for example, data that changes every week) and when it doesn't (a one-off job, or data that must not leave your computer).

## Repeat it in ChatGPT

1. In your ChatGPT project (or, without one, a new chat with the same files attached), attach `copperleaf/invoices.csv`, `copperleaf/policies/credit-and-collections-policy.md` and your checked `step-01-first-whole-job/work/claude/payment-matches.csv` (or your `work/chatgpt/` copy, if you work only in ChatGPT).
2. Paste the prompts from instructions 3, 5, 6 and 7 in turn, changing `work/claude/` to `work/chatgpt/` and asking for each file to download.
3. Download the files into `work/chatgpt/`, open each one, and run the same checks.
4. In `NOTES.md`, compare: did both apps get the same band totals? Which made the better sheet, memo and slides, and why? Where did each app save the files before you downloaded them?

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

> 💡 Working only in ChatGPT? Later steps read files you made here, such as `step-02-three-deliverables/work/claude/figures.csv`. Wherever a step names a file in a `work/claude/` folder, use your copy in the matching `work/chatgpt/` folder instead (and the other way round if you work only in Claude).

## Check it

- [ ] **The grand total, by hand.** In `figures.csv`, add up the open amounts yourself. It must equal the total Claude reported in instruction 3, and the grand total in the sheet.
- [ ] **Three ages, by hand.** Pick three invoices: one not yet due, one in 1 to 30 days and one of the oldest. Work out each one's days overdue yourself from its due date to 2 November 2026, and check its band.
- [ ] **The payments really were applied.** Pick two invoices that a matched payment paid last week. Neither should appear as open.
- [ ] **The disputed invoice is on its own line,** and is not counted as overdue in the bands.
- [ ] **The sheet uses formulas.** Click a band total on the Summary sheet. The formula bar shows a formula, not a typed number.
- [ ] **All three agree.** The total owed and the overdue total are the same in the sheet, the memo and the slides.
- [ ] **Every policy claim in the memo is right.** Open the policy at each section the memo cites and check it says that.

## Keep it

Do this last, after the ChatGPT run and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-02: three deliverables` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-02-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/claude/` with `figures.csv`, `aged-receivables.xlsx`, `overdue-memo.docx` and `monday-slides.pptx`
- [ ] `work/chatgpt/` with ChatGPT's three files (or a transfer plan in `NOTES.md`)
- [ ] `work/my-checks.md` with your three hand-worked totals and the result of every check
- [ ] **Checked:** the grand total and three ages worked out by you, and the same figures in all three deliverables
- [ ] `work/memo-rounds.md`: at least two rounds, each with its grade, and a second AI's review
- [ ] `NOTES.md`: how the apps compared, and where each saved its files
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] Optional: `work/dashboard-note.md`
- [ ] Committed, tagged `step-02-done` and pushed

## References

- [Build Something](https://agentfactory.panaversity.org/claude-and-chatgpt-2/build-something/overview/) and [One job, three deliverables](https://agentfactory.panaversity.org/claude-and-chatgpt-2/build-something/one-job-three-deliverables/)
- [Use skills in Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude) (Anthropic): how Claude makes sheets, documents and slides
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md), sections 4 and 5

---

[← Step 01: Your First Whole Job](../step-01-first-whole-job/) · [Roadmap](../README.md#roadmap) · [Step 03: Behind the Screen: A Safe Desk for the Work →](../step-03-behind-the-screen/)
