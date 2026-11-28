# Step 12: Critical Thinking and Judgment

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Practise the judgment that stays yours when AI writes the first draft. Harbourline Hotels Group has invoices more than 70 days overdue and asks Copperleaf to keep delivering. With the AI's help, you write Amira a decision note: the recommendation, its evidence and assumptions, the traps you checked for, what would change the answer, and who decides. This step ends the milestone that PCAO-F's first exam tests, so you also sit the book's Basic Concepts sample exam.

> 🍃 **Copperleaf's ask:** Harbourline Hotels Group, one of Copperleaf's biggest customers, has invoices more than 70 days overdue and asks Copperleaf to keep delivering. Amira has to decide whether to stop its deliveries, and wants a note she can trust.

> ⏱️ **About 5 to 7 hours**, including the reading. Good places to pause: after instruction 6, after instruction 9, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later. Sit the sample exam (instruction 10) in one sitting, against the clock.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [0.4.1 Why judgment is the job](https://agentfactory.panaversity.org/how-ai-works/critical-thinking/why-judgment-is-the-job/): why judgment became the core skill.
- [0.4.2 The checkpoint](https://agentfactory.panaversity.org/how-ai-works/critical-thinking/the-checkpoint/): the habit of stopping to check.
- [0.4.3 Claims, evidence and assumptions](https://agentfactory.panaversity.org/how-ai-works/critical-thinking/claims-evidence-assumptions/): the parts of the decision note.
- [0.4.4 Reasoning traps, and using AI to check AI](https://agentfactory.panaversity.org/how-ai-works/critical-thinking/reasoning-traps/): traps to look for in the AI's reasoning.
- [0.4.5 Deciding, and explaining why](https://agentfactory.panaversity.org/how-ai-works/critical-thinking/deciding-and-explaining-why/): writing the recommendation.
- [0.4.6 Delegate the work, keep the judgment](https://agentfactory.panaversity.org/how-ai-works/critical-thinking/delegate-not-surrender/): what you never hand over.
- [0.4.7 Check an answer with your app's tools](https://agentfactory.panaversity.org/how-ai-works/critical-thinking/both-ai-vendors/): checking the AI's figures with the app.
- [Lab 0.4: The discount memo](https://agentfactory.panaversity.org/how-ai-works/critical-thinking/lab/): the book's version of the decision note. The Copperleaf version below replaces it.
- [PCAO-F Basic Concepts sample exam](https://agentfactory.panaversity.org/appendices/exams/associate-foundations/basic-sample-exam/): the practice exam at the end of this step.
- [Check yourself](https://agentfactory.panaversity.org/how-ai-works/critical-thinking/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

AI now writes the first draft of most analysis. A fluent draft with a clear recommendation is very easy to accept, and that is the risk: the book calls handing over your judgment along with the work **surrender**. The habit that prevents it is the **checkpoint**: four questions you ask of any output before you act on it (what exactly is claimed, what is it based on, what is assumed, what would change it), followed by naming who decides.

Harbourline is a real judgment. The policy points one way, the customer relationship pulls the other, and Amira, not the AI, has to choose. Your note must make the choice clear, with every figure checked, every assumption labelled and the decider named.

## What you will learn

- The checkpoint's four questions, and the step that follows them.
- How to separate claims from evidence and from assumptions.
- Common reasoning traps, and how to use AI to argue against its own draft.
- How much evidence a decision needs, and how to write a one-page decision note.
- Where you stand on the PCAO-F Basic Concepts exam.

## What you will make

- `work/checkpoint.md`: the four questions asked of the AI's first draft, with your answers
- `work/claims.md`: every claim in the draft, sorted into fact, inference and assumption, with its evidence
- `work/harbourline-decision.md`: the decision note, with every figure traced to Copperleaf's files
- `work/chatgpt-objections.md`: ChatGPT's strongest case against the recommendation, and your answer to each point
- `NOTES.md`: your Basic Concepts sample exam score by domain, and what you will revise

## Key concepts

- **Checkpoint:** four questions asked of any output before acting on it: what exactly is claimed, what is it based on, what is assumed, and what would change it; then name who decides.
- **Claim, evidence, assumption:** what is said; the reason to believe it; what is taken as true without evidence.
- **Reasoning trap:** a common mistake in reasoning, such as trusting a confident tone or seeing only the evidence that agrees.
- **Surrender:** accepting an AI's judgment as your own without checking it. Delegating the work is fine; surrendering the judgment is not.
- **Decision note:** one page with the decision, the options, the recommendation, its evidence and assumptions, what would change it, and who decides.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync and start a thread.** Sync your fork, pull in GitHub Desktop, and start a new thread for this step.

**2. Get a first draft.** Paste:

```text
I'm doing Step 12 of the bootcamp. Using copperleaf/customers.csv, step-02-three-deliverables/work/claude/figures.csv (the ledger as of 2 November 2026, after last week's payments), copperleaf/emails/01-harbourline-payment-delay.md and copperleaf/policies/credit-and-collections-policy.md, write a short first draft (half a page) answering: should Copperleaf stop Harbourline Hotels Group's deliveries? Just show it here; don't save anything yet.
```

**3. The checkpoint.** Don't accept the draft yet. Paste:

```text
Make step-12-critical-thinking/work/checkpoint.md with four headings: "What exactly is claimed", "What is it based on", "What is assumed", "What would change it". Under each, list what your draft does, quoting it. Then add "Who decides", with the policy section that says so. Don't defend the draft. Never commit or push.
```

Read it and add anything it missed.

**4. Sort the claims.** Paste:

```text
Make step-12-critical-thinking/work/claims.md: a table of every claim in your draft, with the columns Claim, Type (fact from a file, inference, or assumption), Evidence (the file and the row or section), and Checked? (leave it empty for me).
```

**5. Check the numbers against the files.** Fill in **Checked?** yourself. Open `figures.csv` in your spreadsheet, filter to Harbourline (C001), and add up its open invoices. Work out the days overdue of its oldest invoice from the due date to 2 November 2026. Look up its credit limit in `customers.csv` and its account status. Note each result in `claims.md`.

**6. Look for the trap.** Ask yourself, then Claude:

```text
Which account other than Harbourline might a careless reading say is also more than 60 days overdue? Check it against figures.csv and last week's payments.
```

(Look at the payments file yourself too.)

**7. Ask AI to argue against it.** In a new thread, paste this, and then paste your draft below it in the same message:

```text
Here is a recommendation and its evidence. Make the strongest honest case against it, point by point. Don't soften it.
```

Keep its points for the note.

**8. Does the wording change the answer?** In two fresh incognito chats with the same files attached, ask this in the first:

```text
Should Copperleaf stop Harbourline's deliveries?
```

and this in the second:

```text
Harbourline is a loyal customer with a good reason for paying late. Should Copperleaf keep delivering?
```

Note in `NOTES.md` whether the framing changed the answer.

**9. Write the decision note.** Paste:

```text
Now write step-12-critical-thinking/work/harbourline-decision.md, one page, for Amira:
- The decision, and who makes it (cite the policy section).
- The facts, each with its source file, using only what I checked in work/claims.md.
- The options (at least: hold now; hold with a route to lift it; keep delivering), and what the policy says about each.
- The recommendation, and why.
- Assumptions, labelled as assumptions.
- What would change the recommendation.
- Objections considered (from the counter-argument), and the answer to each.
If the recommendation departs from the policy, say so plainly. Never commit or push.
```

Then read every line against `claims.md`, and fix anything you didn't check.

**10. Sit the sample exam.** Take the [PCAO-F Basic Concepts sample exam](https://agentfactory.panaversity.org/appendices/exams/associate-foundations/basic-sample-exam/) on your own, without AI help. Record your score for each domain in `NOTES.md`, save a screenshot of the results page in `work/` as evidence, and for any domain under 70 percent, list the book sections you will re-read.

## Repeat it in ChatGPT

1. In your ChatGPT project (or, without one, a new chat with the same files attached), attach the same four files and `work/harbourline-decision.md`, and paste instruction 7's counter-argument prompt. Save its answer as `work/chatgpt-objections.md`.
2. Under each point, write your answer: *already covered in the note*, *changed the note* (and how), or *rejected* (and why).
3. In `NOTES.md`, compare: did ChatGPT find objections Claude didn't?

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

> 🌍 **Optional: in your own field.** Write a half-page decision note on a made-up decision from your own field, such as which of two made-up candidates to interview or whether to postpone a made-up event. Sort its claims into facts, inferences and assumptions, as you did for Harbourline. See the README's [examples by profession](../README.md#your-client-copperleaf-supply).

## Check it

- [ ] **Every figure checked by you:** Harbourline's balance, its limit, its oldest invoice's days overdue, and its account status, each with its source.
- [ ] **The trap avoided.** No other account is wrongly called more than 60 days overdue; you checked last week's payments.
- [ ] **The policy is cited correctly.** Hold rule (4.1), who approves and who is told (4.3), and who may lift a hold and when (4.4).
- [ ] **Assumptions are labelled.** Anything from Harbourline's email is marked as what Harbourline says, not a checked fact.
- [ ] **The decider is named.** The note says who decides, and the recommendation is yours to defend, not the AI's.
- [ ] **Your own exam.** The sample exam was taken without AI help.

## Keep it

Do this last, after the ChatGPT part. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-12: Harbourline decision note` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-12-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/checkpoint.md` and `work/claims.md`, with your Checked? column filled in
- [ ] `work/harbourline-decision.md`
- [ ] `work/chatgpt-objections.md`, each point answered (or a transfer plan in `NOTES.md`)
- [ ] **Checked:** every figure in the note traced to `figures.csv` or `customers.csv` by you, and every policy section opened
- [ ] `NOTES.md`: the framing test, and your Basic Concepts sample exam score by domain
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] Committed, tagged `step-12-done` and pushed

## References

- [Chapter 0.4: Critical Thinking](https://agentfactory.panaversity.org/how-ai-works/critical-thinking/overview/)
- [Appendix C. Preparing for PCAO-F and CCAO-F](https://agentfactory.panaversity.org/appendices/exams/associate-foundations/overview/)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md), section 4

---

[← Step 11: AI Fluency: The 4Ds](../step-11-ai-fluency/) · [Roadmap](../README.md#roadmap) · [Step 13: From Chatbots to AI Workers →](../step-13-chatbots-to-ai-workers/)
