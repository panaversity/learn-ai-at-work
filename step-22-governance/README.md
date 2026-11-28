# Step 22: Governance and Responsible Use

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Decide what the Receivables Worker should and should not do, and what may never go into it. You rate each proposed use as appropriate, appropriate with review or inappropriate, checking it against the vendors' usage policies, set the rules for customer and bank data (de-identified before upload), name who owns, approves and removes each piece of knowledge, and mark the points where a person must sign before anything leaves Copperleaf.

> 🍃 **Copperleaf's ask:** Copperleaf's bank asked how it uses AI with customer data. Amira wants a written policy she can send, and a record that shows the team follows it.

> ⏱️ **About 6 to 8 hours**, including the reading. Good places to pause: after instruction 4, after instruction 7, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

> 🧭 **Your prompts in this step: Construct.** For each task, the step says what your prompt must ask for. Write the prompt yourself first, then open the example under it, compare, and use whichever is better. Every good prompt here names its files, the as-of date where it matters, where to save, and ends with *never commit or push*; anything that drafts for a customer adds *draft only, send nothing*. Keep the prompts you wrote in `NOTES.md`.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [10.1 Should it do this, and who does it affect?](https://agentfactory.panaversity.org/managing-ai-workers/governance-and-responsible-use/appropriate-use/): rating each proposed use.
- [10.2 Can this data go in, and by which route?](https://agentfactory.panaversity.org/managing-ai-workers/governance-and-responsible-use/can-this-data-go-in/): the data rules.
- [10.3 Ownership, approval and takedown of knowledge](https://agentfactory.panaversity.org/managing-ai-workers/governance-and-responsible-use/ownership-and-takedown/): owners and takedown for the KSoR.
- [10.4 Before it leaves: who signs, and who can open it](https://agentfactory.panaversity.org/managing-ai-workers/governance-and-responsible-use/when-a-human-must-sign/): where a person signs.
- [10.5 The first hour, the policy and the record](https://agentfactory.panaversity.org/managing-ai-workers/governance-and-responsible-use/organizational-policy/): the policy and the Governance Record.
- [10.6 Carry out the policy in your own app](https://agentfactory.panaversity.org/managing-ai-workers/governance-and-responsible-use/both-ai-vendors/): where the settings that carry out the policy are in Claude and ChatGPT, and what no setting does.
- [Lab 10: yes, on these terms](https://agentfactory.panaversity.org/managing-ai-workers/governance-and-responsible-use/lab/): the book's version of this step. The Copperleaf version below replaces it.
- [Anthropic's Usage Policy](https://www.anthropic.com/legal/aup) and [OpenAI's usage policies](https://openai.com/policies/usage-policies/): outside the book: the vendors' own rules, which you check each proposed use against.
- [Check yourself](https://agentfactory.panaversity.org/managing-ai-workers/governance-and-responsible-use/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

Governing a worker means a named person decides, in writing, four things: whether it should do a job at all, what data may go in, who owns what it knows, and who signs before a result leaves. The book rates each use as **appropriate**, **appropriate with review** (the exam guide calls it "appropriate with safeguards": a defined human check happens before the output is used) or **inappropriate**, by asking five screens and naming the **deciding factor**, the one that would change the answer. It also asks who the output affects, including the people a list leaves out.

Copperleaf's own policy already has rules for AI (section 10). Your job is to turn them into a working **Governance Record** the team keeps, and a one-page policy Amira can send the bank, and to check that the apps' settings actually carry them out. Some things no setting does: a person still has to sign.

## What you will learn

- How to rate a proposed use with the five screens, and name the deciding factor.
- How to decide what data a task needs, remove the rest, and choose an approved route in.
- How to prepare sensitive data for analysis in line with a policy.
- Who owns each piece of knowledge, and how takedown differs from deprecation.
- Which outputs a person must sign, and who may open a result.
- The first hour after data goes where it shouldn't, and how to keep a Governance Record.

## What you will make

- `work/governance-record.md`: uses rated, data rules, knowledge owners and takedown, sign-off points, the first-hour plan, and when to re-check
- `work/de-identified/customers-for-analysis.csv`: a copy of the customer list prepared for analysis as the policy requires, and `work/de-identify-check.md`
- `work/ai-policy-for-the-bank.md`: a one-page AI policy for Amira to send the bank
- `work/settings-check.md`: the settings in each app that carry out the policy, and what no setting does
- `work/role-contract.md`: version 9, pointing to the Governance Record
- `NOTES.md`: how the apps compared

## Key concepts

- **Appropriate, appropriate with review, inappropriate:** the three answers for a proposed use; with review means a defined human check before the output is used.
- **Deciding factor:** the screen that, if its answer changed, would move the use into another category.
- **De-identify:** remove or replace everything that identifies a person or company before data goes to an AI tool, without breaking the task.
- **Takedown:** removing knowledge, and every served copy of it, because it must not be used at all; unlike deprecation, which replaces it with a successor.
- **Governance Record:** the written record of these decisions, who made them and when, kept and re-checked.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync, start a thread, and bring the living documents forward.** Sync your fork, pull in GitHub Desktop, start a new thread for this step, and paste:

```text
I'm doing Step 22 of the bootcamp. Copy step-21-recurring-work/work/role-contract.md, authority-envelope.md and the ksor folder to step-22-governance/work/, unchanged. Never commit or push.
```

**2. Rate six proposed uses.** Write a prompt for a "Uses" section in `work/governance-record.md` that rates these six proposed uses with chapter 10.1: (1) drafting the weekly reminder list; (2) deciding which accounts go on hold; (3) scoring customers' creditworthiness from their payment history to set new credit limits; (4) summarising customer emails for Ben; (5) replying directly to customers' payment questions; (6) ranking which overdue customers to chase first. Your prompt works if every rating has its deciding factor, every "with review" names the human check, and each use says who its output affects, including anyone left out.

<details>
<summary>Compare with an example prompt</summary>

```text
Using chapter 10.1 of The AI Agent Factory, start step-22-governance/work/governance-record.md with a section "Uses". Rate each of these proposed uses of the Receivables Worker as appropriate, appropriate with review, or inappropriate, with the five screens, the deciding factor and, for "with review", the human check:
1. Drafting the weekly reminder list.
2. Deciding which accounts go on hold.
3. Scoring customers' creditworthiness from their payment history, to set new credit limits.
4. Summarising customer emails for Ben.
5. Replying directly to customers' payment questions.
6. Ranking which overdue customers to chase first.
Also say, for each, who the output affects, including anyone a list leaves out. Never commit or push.
```

</details>

Then open [Anthropic's Usage Policy](https://www.anthropic.com/legal/aup) and [OpenAI's usage policies](https://openai.com/policies/usage-policies/) and check each use against them yourself. Note in the record anything they say about decisions that affect people's or businesses' access to credit or services. Change any rating you now disagree with, and say why.

**3. What data may go in.** Write a prompt for a "Data" section, using chapter 10.2 and Copperleaf's policy section 10. Your prompt works if the section settles what the weekly run needs, what must never go in, and which routes in are approved for which data, and by whom.

<details>
<summary>Compare with an example prompt</summary>

```text
Add a section "Data" to governance-record.md, using chapter 10.2 and Copperleaf's policy section 10: for the weekly run, what data the job actually needs, what it doesn't, what must never go in (bank details), and how contact details are handled (10.2). For each route in (upload to a project, a connector, pasting into a chat), say whether it is approved for that data, and who approves.
```

</details>

**4. Prepare sensitive data for analysis.** Imagine Rosa wants an analysis of payment behaviour, and Copperleaf's tools are not approved for contact details. Write a prompt for `work/de-identified/customers-for-analysis.csv`, made from `copperleaf/customers.csv`, and for `work/de-identify-check.md`. Your prompt works if the new file keeps only what the analysis needs, contains no names or contact details, leaves the original unchanged, and the check note gives the policy reason for each removal.

<details>
<summary>Compare with an example prompt</summary>

```text
Make step-22-governance/work/de-identified/customers-for-analysis.csv from copperleaf/customers.csv: keep customer_id, type, credit_limit, payment_terms_days and account_status; remove name, contact_role and contact_email. Don't change the original. Then write step-22-governance/work/de-identify-check.md: what you removed and why (policy 10.2), and whether the analysis can still be done with customer_id alone.
```

</details>

Open the new file and check yourself that no name or email address is left.

**5. Who owns what it knows.** Add a section "Knowledge owners" (10.3): for each KSoR concept, its owner, who approves a change, and how a takedown would remove every served copy (the projects in both apps, any connector folder, skills).

**6. Who signs, and who can open it.** Add a section "Before it leaves" (10.4): every output that may leave Copperleaf (reminders, final notices, statements, the bank summary, this policy), who signs it, and who may open it. Check each against policy sections 5.1 and 11.

**7. The first hour.** Add a section "The first hour" (10.5): the five steps if a customer's bank details were pasted into an AI chat by mistake, who is told, and how you'd tell a policy gap from a training gap or a lapse.

**8. Write the policy for the bank.** Write a prompt for `work/ai-policy-for-the-bank.md`, one page from Amira to the bank. Your prompt works if a bank manager with no AI knowledge could follow it, every statement matches `governance-record.md` and policy section 10, and it claims nothing you haven't done.

<details>
<summary>Compare with an example prompt</summary>

```text
Write step-22-governance/work/ai-policy-for-the-bank.md, one page from Amira to Copperleaf's bank, in plain words: what Copperleaf uses AI for (and doesn't), what data may and may not go in, who checks AI work and who signs anything that leaves the company, how knowledge is approved, and what happens if something goes wrong. Every statement must match governance-record.md and copperleaf/policies/credit-and-collections-policy.md section 10. Claim nothing we haven't done.
```

</details>

Check every sentence against the record and the policy.

**9. Check the settings.** Read [10.6](https://agentfactory.panaversity.org/managing-ai-workers/governance-and-responsible-use/both-ai-vendors/), then open Claude's settings (privacy, memory, connectors, sharing) and write in `work/settings-check.md` which settings carry out which rule of the policy, and which rules no setting can carry out.

**10. Draft 9 of the contract.** Write a prompt that adds the Governance Record to `work/role-contract.md` as Draft 9. Your prompt works if only the part it belongs in changes, and the Change log records the draft, the date and who must approve it.

<details>
<summary>Compare with an example prompt</summary>

```text
In step-22-governance/work/role-contract.md, add the Governance Record under What bounds it, and a Change log line with today's date, approved by Rosa (pending): "Draft 9: governance, from step 22". Change nothing else.
```

</details>

Add a "Re-check" line at the end of `governance-record.md`: when it is reviewed next, and by whom.

## Repeat it in ChatGPT

1. In your ChatGPT project (or, without one, a new chat with the same files attached), attach `governance-record.md` and `ai-policy-for-the-bank.md`, and ask:

   ```text
   Review this AI policy as the bank's risk officer would. List every statement that is vague, unsupported by the Governance Record, or promises more than a setting or a person can deliver.
   ```

   Save the answer as `work/chatgpt-policy-review.md`, mark each point, and make accepted changes in Claude.
2. Open ChatGPT's own settings and add a "ChatGPT" section to `settings-check.md`.

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

> 🌍 **Optional: in your own field.** Rate three AI uses from your own field (for example, a teacher: drafting a quiz, grading essays, emailing parents) as appropriate, appropriate with review or inappropriate, with the deciding factor for each. Describe them in general terms, with no real people or data. See the README's [examples by profession](../README.md#your-client-copperleaf-supply).

## Check it

- [ ] **Every use rated,** with the five screens, a deciding factor, and the vendors' policies checked by you.
- [ ] **No bank details,** and no contact details where the route isn't approved for them (policy 10.2).
- [ ] **The de-identified file is clean.** You opened it: no names, no email addresses.
- [ ] **Every concept has an owner** and a takedown path that reaches every copy.
- [ ] **Every outward output has a signer,** matching policy sections 5.1 and 11.
- [ ] **The bank policy claims only what's true,** sentence by sentence.

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-22: governance record and AI policy` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-22-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/governance-record.md`, with its six sections and a re-check date
- [ ] `work/de-identified/customers-for-analysis.csv` and `work/de-identify-check.md`
- [ ] `work/ai-policy-for-the-bank.md` and `work/chatgpt-policy-review.md` (or a transfer plan in `NOTES.md`)
- [ ] `work/settings-check.md`, for both apps
- [ ] `work/role-contract.md` (Draft 9)
- [ ] **Checked:** every use checked against both vendors' usage policies, the de-identified file opened, and every sentence of the bank policy traced to the record or the policy
- [ ] `NOTES.md`: how the apps compared
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] `NOTES.md`: the prompts you wrote yourself for this step
- [ ] Committed, tagged `step-22-done` and pushed

## References

- [Chapter 10: Governance and Responsible Use](https://agentfactory.panaversity.org/managing-ai-workers/governance-and-responsible-use/overview/)
- [Anthropic's Usage Policy](https://www.anthropic.com/legal/aup) and [OpenAI's usage policies](https://openai.com/policies/usage-policies/)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md), sections 10 and 11

---

[← Step 21: Work That Runs Without You](../step-21-recurring-work/) · [Roadmap](../README.md#roadmap) · [Step 23: When the Worker Goes Wrong →](../step-23-when-it-goes-wrong/)
