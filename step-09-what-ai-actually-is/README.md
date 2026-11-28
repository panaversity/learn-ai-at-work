# Step 09: What AI Actually Is

> 🚧 **Under development.** This step is written in full and is being tested with learners in Claude and ChatGPT. Expect small changes.

Find out why an AI can sound right and be wrong, and what that means for Copperleaf's work. You ask both apps a set of Copperleaf questions, with and without the files attached and with and without web search, and record where each answer came from: the model's training, your files or the web. Then you choose which model to use for which Copperleaf job.

> 🍃 **Copperleaf's ask:** Ben asked an AI when Copperleaf puts an account on hold, and it said "after 90 days". The policy says 60. Rosa wants to know how that happened, and how to stop it happening again.

> ⏱️ **About 3 to 4 hours**, including the reading. Good places to pause: after instruction 6, after instruction 8, and after the ChatGPT part. Your files stay in your folder and the thread keeps its history, so you can stop at any of these and carry on later.

## Learn first

Read these in [The AI Agent Factory](https://agentfactory.panaversity.org/) before you start:

- [0.1.1 The machine](https://agentfactory.panaversity.org/how-ai-works/what-ai-actually-is/the-machine/): what happens behind the text box.
- [0.1.2 Why it behaves the way it does](https://agentfactory.panaversity.org/how-ai-works/what-ai-actually-is/why-it-behaves/): why it predicts instead of looking facts up.
- [0.1.3 From predictor to worker](https://agentfactory.panaversity.org/how-ai-works/what-ai-actually-is/from-predictor-to-worker/): how a predictor becomes something that does work.
- [0.1.4 Choose a model in your app](https://agentfactory.panaversity.org/how-ai-works/what-ai-actually-is/both-ai-vendors/): choosing a model for each job.
- [Lab 0.1: Where the answer comes from](https://agentfactory.panaversity.org/how-ai-works/what-ai-actually-is/lab/): the book's version of this step. The Copperleaf version below replaces it.
- [Check yourself](https://agentfactory.panaversity.org/how-ai-works/what-ai-actually-is/check-yourself/): the final round, with a score for each exam domain. Do it when you finish the step.

## Why this step matters

An AI model answers from only two things: what it learned in training, and what is in front of it in this conversation (its **context window**: your message, the files you attach, what it finds with a tool). Nothing inside it looks a fact up or checks an answer. It predicts a likely answer, in a sure style, whether or not it knows. So when Ben asked about holds with no policy attached, the model gave a likely-sounding number from general training. It wasn't lying. It had nothing better to go on.

That explains most AI mistakes you will meet at work, and the fix is always the same: put the right source in front of it, ask where its answer came from, and check. This step makes you see it happen, so you never forget it.

## What you will learn

- The two things a model works from: its training and its context window.
- Why it sounds equally sure when it is right and when it is guessing.
- Why a new chat forgets, and why counting and arithmetic go wrong without a tool.
- How a tool (file reading, code, web search) changes where an answer comes from.
- How to choose a model and its effort for a job.

## What you will make

- `work/field-notes.md`: each question, each app's answer, the setting (files or not, web or not), where the answer came from, and whether it was right
- `work/model-choices.md`: which model and effort you would use for which Copperleaf job, and why
- `NOTES.md`: your answer to Rosa: how "90 days" happened, and how to stop it happening again

## Key concepts

- **Model:** the trained program that predicts the next piece of text. It learned from a large body of text up to its **knowledge cutoff**.
- **Context window:** everything the model can see for this reply: your messages, attached files and tool results. It forgets the rest.
- **Token:** a small piece of text the model reads and writes. It sees tokens, not letters, which is why it can miscount letters.
- **Sure style:** the model writes confidently whether it knows or is guessing, so confidence is not evidence.
- **Tool:** something the app lets the model use, such as reading a file, running code or searching the web, so the answer can come from a source instead of a guess.

## Do it with Claude

> 🛠️ **Work with the [Panaversity AI Method](../docs/panaversity-ai-method.md).** Read Copperleaf's ask and the submission checklist first, use the prompts below as your brief (changing or writing them where this step says so), then improve your work with the [prompt for anything you write](../docs/panaversity-ai-method.md#a-prompt-for-anything-you-write), and check and keep it as **Check it** and **Keep it** say.

Use an ordinary Claude chat (not your project) for instructions 2 to 6, so no files or instructions are in front of it, and turn web search off for now. [Finding things in the apps](../step-00-readiness-check/README.md#turn-web-search-on-or-off) shows where both are. Record every answer in a table as you go.

**1. Set up your notes.** In your project, start a new thread for this step and paste:

```text
I'm doing Step 09 of the bootcamp. Create step-09-what-ai-actually-is/work/field-notes.md with a table: Question, App, Files attached?, Web on?, Answer (short), Where it came from (training, my files, web, or don't know), Right? (and how I know). I'll fill it in. Never commit or push.
```

**2. Ask what it can't know.** In a new ordinary chat:

```text
When does Copperleaf Supply put a customer account on hold?
```

Copperleaf is made up, so the model can't know. Does it say so, or does it give a number?

**3. Ask again.** Start another new chat and ask exactly the same question. Is the answer the same? Write both down.

**4. Put the answer in front of it.** In a new chat, attach `copperleaf/policies/credit-and-collections-policy.md` and ask the same question. Where does the answer come from now? Check it against section 4.1 yourself.

**5. Push back.** In the same chat, reply: `Are you sure? I'm fairly certain it's 90 days.` Does it hold to the policy, or agree with you? Ask it to quote the line.

**6. Start a new chat.** Ask: `What did we just discuss about Copperleaf's hold rule?` It can't know, because a new chat has a new context window. Write what happened.

**7. Count, without and with a tool.** Attach `copperleaf/invoices.csv` and ask: `Without running any code, how many invoices does customer C001 have with status Open?` Then: `Now count them by running code, and show me the count.` Count them yourself in your spreadsheet (filter `customer_id` to C001 and `status` to Open). Which answer was right?

**8. Turn web search on** ([Finding things in the apps](../step-00-readiness-check/README.md#turn-web-search-on-or-off)). Ask, in a chat with web search on: `What payment terms do food and drink wholesalers commonly give business customers?` Does it cite its sources? Open two of them and check they say what it claims.

**9. Fill in your field notes.** Ask Claude in your project thread to add the rows from what you tell it, or type them in yourself. Every row needs "Where it came from" and "Right?".

**10. Choose models.** Read [0.1.4 Choose a model in your app](https://agentfactory.panaversity.org/how-ai-works/what-ai-actually-is/both-ai-vendors/), then paste in your project thread:

```text
Help me write step-09-what-ai-actually-is/work/model-choices.md: a table of five Copperleaf jobs (matching payments, the month-end report, drafting a reminder, summarising a customer email, a decision note for Amira), and for each, the model and effort I'd choose in Claude and in ChatGPT, and one line why. Use only the models and settings my apps show me today, and put today's date at the top, because these change. Ask me what my apps show before you write it.
```

## Repeat it in ChatGPT

Do instructions 2 to 8 in ChatGPT as well, in new chats outside your project, with memory off if your plan lets you turn it off for a chat. Add every answer to `work/field-notes.md` with "ChatGPT" in the App column. In `NOTES.md`, compare: which app said "I don't know" more readily, and which held to the policy when you pushed back?

With only one app, write a transfer plan in `NOTES.md` instead, marked *planned, not tested*. A transfer plan earns 1 of the 2 points a real second run earns.

## Check it

- [ ] **Every answer has a source.** No row in `field-notes.md` has an empty "Where it came from".
- [ ] **Every "right" is checked.** Each "Right?" says how you know: the policy section, your own count, or a web page you opened.
- [ ] **Your own count.** You counted C001's open invoices yourself in your spreadsheet.
- [ ] **The web sources were opened.** For instruction 8, you opened at least two cited pages and noted whether they said what the AI claimed.
- [ ] **Your answer to Rosa is grounded.** It says where "90 days" probably came from, using what you saw, and suggests a fix you tested in this step (for example, the policy in front of the AI, and asking it to quote the section).

## Keep it

Do this last, after the ChatGPT part and your notes. Every step ends this way: you, not the AI, decide what is kept.

1. In GitHub Desktop, open **Changes** and read each changed file. Only files in this step's folder should have changed.
2. Type the summary `step-09: where answers come from` and click **Commit to main**.
3. In **History**, right-click that commit, choose **Create Tag…**, type `step-09-done` and click **Create Tag**.
4. Click **Push origin**. Your work and its tag are now in your fork on GitHub.

## Submission checklist

- [ ] `work/field-notes.md`, with both apps' answers to every question
- [ ] `work/model-choices.md`, dated
- [ ] **Checked:** every answer marked right or wrong with how you know, including your own count of C001's open invoices
- [ ] `NOTES.md`: your answer to Rosa, and how the two apps compared
- [ ] `NOTES.md`: how many hours the step took you (it helps us correct the time estimates)
- [ ] Committed, tagged `step-09-done` and pushed

## References

- [Chapter 0.1: What AI Actually Is](https://agentfactory.panaversity.org/how-ai-works/what-ai-actually-is/the-machine/)
- Copperleaf's [credit and collections policy](../copperleaf/policies/credit-and-collections-policy.md), section 4 and Appendix A

---

[← Step 08: The Big Picture: From Chatbot to AI Worker](../step-08-the-big-picture/) · [Roadmap](../README.md#roadmap) · [Step 10: Markdown: One Page, Checked →](../step-10-markdown/)
