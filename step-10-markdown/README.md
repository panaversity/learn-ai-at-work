# Step 10: Markdown: One Page, Checked

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Learn the simple language AI reads and writes. You turn Copperleaf's long credit and collections policy into a clean one-page Markdown summary, mark every rule with the policy section it came from, check each one line by line, and keep the page as a file the team can use.

> 🍃 **Copperleaf's ask:** Copperleaf's credit policy is a long document that few people read to the end. Rosa wants a one-page version the team and the AI can both use, and proof that it says what the full policy says.

> ⏱️ **About 3 to 4 hours**, including the reading. Good places to pause: after instruction 3, after instruction 5, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [0.2.1 Markdown going in](https://agentfactory.panaversity.org/how-ai-works/markdown/markdown-going-in/): the marks for headings, lists and tables.
- [0.2.2 What comes back](https://agentfactory.panaversity.org/how-ai-works/markdown/what-comes-back/): reading the Markdown the AI writes.
- [0.2.3 A copy you can check](https://agentfactory.panaversity.org/how-ai-works/markdown/one-short-specification/): checking a page line by line against its source.
- [0.2.4 Keep a page as a file in your app](https://agentfactory.panaversity.org/how-ai-works/markdown/both-ai-vendors/): saving the page as a file.
- [Lab 0.2: One page, checked](https://agentfactory.panaversity.org/how-ai-works/markdown/lab/): the book's version of this step. The Copperleaf version below replaces it.
- [Check yourself](https://agentfactory.panaversity.org/how-ai-works/markdown/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

Every AI reply is Markdown: plain text with a few marks, like `#` for a heading, `-` for a list item and `|` for a table. The app turns the marks into a neat page. That matters for two reasons. First, the marks show the model the shape of what you give it, so a policy written as Markdown, with headings and numbered rules, is easier for it to use correctly. Second, **a neat page is only as right as its lines**. A summary that looks clean can still drop a condition, change a number or quote a rule that was replaced.

Copperleaf's policy has a trap for summaries: Appendix A lists the old rules, so a careless summary can pick up a superseded number. A summary in which every line names its section is one you can check, and one the AI can be held to.

## What you will learn

- The handful of Markdown marks you need: headings, lists, bold, tables and links.
- How the same Markdown looks in an app and in a plain text box.
- How to ask for a copy in the shape its next reader needs.
- How to check a summary line by line against its source.
- How to keep a page as a `.md` file and use it in a new chat.

## What you will make

- `work/credit-policy-summary.md`: the one-page summary, each rule marked with the policy section it came from
- `work/policy-check.md`: your line-by-line check, and anything you corrected
- `work/chatgpt-summary.md`: ChatGPT's summary, checked the same way
- `NOTES.md`: what you learned about Markdown, and how the summary did in a new chat

## Key concepts

- **Markdown:** plain text with a few marks for a page's shape: `#` headings, `-` lists, `**bold**`, `|` tables.
- **Rendered:** shown as a neat page by the app. The same text in a plain box shows the marks.
- **Source mark:** the policy section a rule came from, written next to it, such as "(4.1)".
- **Superseded rule:** a rule that has been replaced and must not be used; Copperleaf lists them in Appendix A.
- **Line-by-line check:** comparing each line of a copy with its source, one at a time, and marking it confirmed or wrong.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync and start a thread.** Sync your fork, pull in GitHub Desktop, and start a new thread for this step.

**2. See the marks.** Paste:

```text
I'm doing Step 10 of the bootcamp. Show me last week's five largest payments from copperleaf/payments-week-44.csv as a Markdown table, with payer, amount and reference. Then show me the same table again inside a code block, so I can see the marks.
```

Copy the first table and paste it into a plain text editor (TextEdit set to plain text, or Notepad). You see the `|` marks. Paste it into a Word or Google document, and you may see a table or a mess. That is the difference between Markdown and what the app shows you.

**3. Ask for the shape the next reader needs.** Paste:

```text
Now give me the same five payments as a simple list Ben could paste into an email, with no table.
```

Notice that the facts must stay the same when the shape changes.

**4. Turn the policy into one page.** Paste:

```text
Read copperleaf/policies/credit-and-collections-policy.md (version 4.0). Write a one-page Markdown summary for Copperleaf's finance team and for AI tools, saved as step-10-markdown/work/credit-policy-summary.md.

Use: a title; one line saying the policy version, effective date and owner; then a heading for each topic (payment terms, credit limits, holds, reminders, disputes and credit notes, write-offs, unmatched payments and refunds, bank-detail changes, AI use, who approves what). Under each, short bullet points, one rule per bullet, each ending with its section in brackets, such as "(4.1)". Every number and every "or" condition must be exactly as the policy says. Do not use anything from Appendix A, which lists superseded rules. Keep it to one page.

Don't change the policy. Never commit or push.
```

**5. Check each rule against the policy.** Open the summary and the policy side by side. Then paste:

```text
Make step-10-markdown/work/policy-check.md: a table with one row for every bullet in the summary, with the columns: Bullet, Section cited, What the policy says there (quote it), Match? Leave the Match? column empty for me.
```

Now fill in **Match?** yourself for every row (*yes*, or what is wrong), reading the quoted line and, for anything that looks off, the policy itself. Don't trust the quote column without looking: the quotes are the AI's too.

**6. Fix it, and see its marks.** For each row that isn't a match, ask Claude to fix that bullet only, naming the row. Then open `credit-policy-summary.md` in a plain text editor and look at its marks. Is every heading a `#` line, and every rule a `-` line?

**7. Use the page in a new chat.** Start a fresh ordinary chat, attach only `credit-policy-summary.md`, and ask three questions: `When is an account put on hold?`, `Who can approve a credit note of 1,800?` and `What are the payment terms?` Check each answer against the full policy. Write the results in `NOTES.md`.

## Repeat it in ChatGPT

1. In your ChatGPT project (or, without one, a new chat with the same files attached), attach the policy and paste the prompt from instruction 4, asking for the file to download. Save it as `work/chatgpt-summary.md`.
2. Check it line by line in the same way, adding a "ChatGPT" section to `work/policy-check.md`.
3. In `NOTES.md`, compare: did either summary drop a condition, change a number or use a superseded rule?

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **Every bullet is checked by you.** Every row of `policy-check.md` has your own Match? entry.
- [ ] **No superseded rule.** Nothing in the summary comes from Appendix A. Check the payment terms, the hold trigger, where credit limits come from, and the Finance Manager's credit-note limit especially.
- [ ] **Every condition is whole.** Both halves of the hold rule in 4.1 are there.
- [ ] **One page,** with the version, effective date and owner at the top.
- [ ] **It works in a new chat.** The three answers in instruction 7 match the full policy.

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-10: one-page policy, checked` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-10-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/credit-policy-summary.md`, each rule marked with its section
- [ ] `work/policy-check.md`, every row checked by you
- [ ] `work/chatgpt-summary.md`, checked the same way (or a transfer plan in `NOTES.md`)
- [ ] **Checked:** every bullet compared with the policy by you, and no Appendix A rule used
- [ ] `NOTES.md`: the new-chat test, and how the two apps compared
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] Committed, tagged `step-10-done` and pushed

## References

- [Chapter 0.2: Markdown](https://agentfactory.panaversity.org/how-ai-works/markdown/overview/)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md)

---

[← Step 09: What AI Actually Is](../step-09-what-ai-actually-is/) · [Roadmap](../README.md#roadmap) · [Step 11: AI Fluency: The 4Ds →](../step-11-ai-fluency/)
