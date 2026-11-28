# Step 08: The Big Picture: From Chatbot to AI Worker

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Step back and see where the work you did in steps 1 to 7 fits in the bigger change the book describes. You redo one piece of Copperleaf's Monday work three ways, the way the Preface shows Maria's invoices: as a chatbot question, as a delegated task, and as a standing responsibility with rules. Then you write Amira a one-page briefing: where Copperleaf stands on the ladder of interaction and the five horizons, what the next rung would ask of it, and which claims about AI products are dated, as the Preface insists. You finish by choosing your own route through the book, the four exams and the ways to earn.

> 🍃 **Copperleaf's ask:** Amira keeps hearing that AI will change how companies like Copperleaf work. Before she spends more money on it, she wants a plain one-page answer: what is changing, where Copperleaf is today, and what comes next.

> ⏱️ **About 3 to 4 hours**, including the reading. Good places to pause: after instruction 2, after instruction 5, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [The Five Horizons: From Agent to Autonomous Economy](https://agentfactory.panaversity.org/five-horizons/): the five steps in the change, and where you stand now.
- [Preface, "The same box, a different machine behind it"](https://agentfactory.panaversity.org/preface/#the-same-box-a-different-machine-behind-it): Maria's invoices done three ways: the pattern you repeat for Copperleaf.
- [Preface, "The ladder of interaction"](https://agentfactory.panaversity.org/preface/#the-ladder-of-interaction): query, message, task, role: the rungs you place Copperleaf on.
- [Preface, "The thesis and five lines"](https://agentfactory.panaversity.org/preface/#the-thesis-and-five-lines): the book's one argument, which your briefing answers for Copperleaf.
- [Preface, "Why certification, governance and earning belong on one path"](https://agentfactory.panaversity.org/preface/#why-certification-governance-and-earning-belong-on-one-path): why this bootcamp joins all three.
- [How to Use This Book](https://agentfactory.panaversity.org/how-to-use-this-book/): choosing your route, and how the labs and Zia Tutor AI help.
- [Certification and Portfolio Roadmaps](https://agentfactory.panaversity.org/certification-and-portfolio-roadmaps/): where PCAO-F sits, and what you build toward.
- [The FDE 2027 Master Plan, "The four-stage FDE certification pathway"](https://agentfactory.panaversity.org/fde-2027-master-plan/#the-four-stage-fde-certification-pathway): Panaversity's four exams in order: this bootcamp prepares you for the first two, PCAO-F Basic and PCAO-F Full.
- [From Skills to Income](https://agentfactory.panaversity.org/from-skills-to-income/overview/): the four ways to earn from these skills, and what each route needs first.

## Why this step matters

You have just done seven steps of real work. This step asks what it adds up to. The book's argument, in its Preface, is that the same text box now leads to very different machines: one that answers a question, one that does a task you hand it, and one that holds a role with rules, week after week. Each rung up does more of the work, and each needs more control. Knowing which rung a job is on tells you how much briefing, limiting and checking it needs.

Owners like Amira hear big promises about AI. Your job is to give a plain, honest answer: what is really changing, where Copperleaf is today, what the next rung would ask of it, and which claims will be out of date by next year. The book dates every claim about a product, because products change monthly; your briefing does the same.

## What you will learn

- The ladder of interaction, and how to place a piece of work on it.
- The five horizons, and where this bootcamp, and Copperleaf, stand on them.
- How to tell a lasting idea from a dated product claim, and how to date a claim.
- The book's routes, the four exams and the four ways to earn, so you can choose your own path.

## What you will make

- `work/three-ways.md`: one piece of Copperleaf's Monday work done as a chatbot question, a delegated task and a standing responsibility, with what your job becomes each time
- `work/briefing-for-amira.md`: a one-page briefing on the ladder and the five horizons for Copperleaf, with every claim about an AI product dated and sourced
- `work/chatgpt-briefing-review.md`: ChatGPT's review of the briefing
- `NOTES.md`: your chosen route through the book, the four exams and one way to earn from these skills

## Key concepts

- **Ladder of interaction:** the rungs from a single answer (query), through a message and a task, to a role held over time; each rung up needs more control.
- **The five horizons:** the book's five stages of change, from a single agent to an autonomous economy.
- **Standing responsibility:** work held as a role, started by its triggers, not by someone asking each time.
- **Dated claim:** a statement about a product's features, prices or limits, written with the date it was true and its source.
- **Route:** the path you choose through the book and the certifications, matched to the work you want to do.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

**1. Sync and start a thread.** Sync your fork, pull in GitHub Desktop, and start a new thread for this step.

**2. One job, three ways.** Choose one piece of Copperleaf's Monday work you already know, such as "find the payments that need a person". Do it three ways, saving what each gives you:

- **As a chatbot question,** in an ordinary chat (outside your project, see [Finding things in the apps](../step-00-readiness-check/README.md#an-ordinary-chat-outside-the-project)) with no files attached: `What should a finance team do with a customer payment that has no invoice reference?`
- **As a delegated task,** in your project thread:

  ```text
  Using copperleaf/payments-week-44.csv, copperleaf/invoices.csv and section 8 of the policy, list last week's payments that need a person, with the reason for each. Save nothing; just show me.
  ```
- **As a standing responsibility,** describe (don't set up) how it would work as a role: paste

```text
Describe, in under 200 words, how "find the payments that need a person" would work as a standing responsibility of an AI worker at Copperleaf: what would start it each week, what it would read, what it may and may not do, who checks it and who it answers to. Don't set anything up.
```

**3. Write the three ways down.** Paste:

```text
Write step-08-the-big-picture/work/three-ways.md: a table with three rows (chatbot question, delegated task, standing responsibility) and the columns: what I typed, what came back, which rung of the ladder of interaction it is (from the book's Preface), and what my job became (asking, checking, or setting limits and reviewing). Base it on what we did in this thread. Never commit or push.
```

Correct anything that isn't what happened.

**4. Draft the briefing for Amira.** Paste:

```text
Draft step-08-the-big-picture/work/briefing-for-amira.md, one page for Copperleaf's owner, in plain words. Sections: "What is changing" (the ladder of interaction and the five horizons, as the book's Preface and Five Horizons pages describe them; quote no more than one short line); "Where Copperleaf is today" (based on what we did in steps 1 to 7 of this bootcamp: which rungs the work is on now); "What the next rung would ask of Copperleaf" (the briefing, limits, checking and an accountable person it would need); and "Claims with a date" (every statement about a specific product's features, price or availability, each with the date and source, or removed). Keep it to one page. Never commit or push.
```

**5. Date every product claim.** Read the draft. For each claim about a product, open the source it gives and check the claim is there and the date is right. Where it has no source, either find one in the book (for example, [Which plan has what](https://agentfactory.panaversity.org/claude-and-chatgpt-2/new-way-of-working/set-up-the-apps/#which-plan-has-what)) or remove the claim. Ask Claude to make only those changes.

**6. Choose your route.** Read How to Use This Book, the Certification and Portfolio Roadmaps, the FDE 2027 Master Plan and From Skills to Income. Then paste:

```text
Ask me five short questions, one at a time, to help me choose my route through The AI Agent Factory: my job, the time I have, whether I want to build or manage, which exam I'm aiming for, and how I'd like to earn. Then suggest a route using only the book's own routes and the four ways to earn, and say which pages you based it on.
```

Write your chosen route in `NOTES.md`, in your own words: the book route, the exams you plan to take and when, and one way to earn you want to try.

## Repeat it in ChatGPT

1. Do instruction 2's chatbot question in ChatGPT too, and add its answer to `three-ways.md`.
2. In your ChatGPT project (or, without one, a new chat with the same files attached), attach `work/briefing-for-amira.md` and paste:

```text
Review this one-page briefing for a company owner. Mark every claim about an AI product that has no date or source, every sentence a non-technical owner wouldn't understand, and anything that promises more than the evidence shows. Don't rewrite it.
```

3. Save the answer as `work/chatgpt-briefing-review.md`, mark each point *accepted* or *rejected*, and make the accepted changes in Claude.

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **The rungs are the book's.** Each rung in `three-ways.md` matches the Preface's ladder of interaction; check each one against the page.
- [ ] **"Where Copperleaf is today" is true.** Everything it says Copperleaf does now is something you did in steps 1 to 7.
- [ ] **Every product claim is dated and sourced,** and you opened each source.
- [ ] **One page, plain words.** Amira could read it in five minutes without asking what a word means.
- [ ] **Your route is yours.** `NOTES.md` explains it in your own words, not the AI's.

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-08: the big picture` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-08-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/three-ways.md` and `work/briefing-for-amira.md`
- [ ] `work/chatgpt-briefing-review.md` (or a transfer plan in `NOTES.md`)
- [ ] **Checked:** every product claim in the briefing opened at its source and dated, and every rung checked against the Preface
- [ ] `NOTES.md`: your route through the book, the exams you plan to take, and one way to earn
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] Committed, tagged `step-08-done` and pushed

## References

- [Preface](https://agentfactory.panaversity.org/preface/) and [The Five Horizons](https://agentfactory.panaversity.org/five-horizons/)
- [How to Use This Book](https://agentfactory.panaversity.org/how-to-use-this-book/), [Certification and Portfolio Roadmaps](https://agentfactory.panaversity.org/certification-and-portfolio-roadmaps/), [The FDE 2027 Master Plan](https://agentfactory.panaversity.org/fde-2027-master-plan/) and [From Skills to Income](https://agentfactory.panaversity.org/from-skills-to-income/overview/)

---

[← Step 07: One Setup for the Month-End](../step-07-month-end-setup/) · [Roadmap](../README.md#roadmap) · [Step 09: What AI Actually Is →](../step-09-what-ai-actually-is/)
