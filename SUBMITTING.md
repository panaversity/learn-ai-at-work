# Submitting Your Work

> 🚧 **Under development.** The rubric and the steps below are planned and will be refined as the bootcamp is tested with learners.

This bootcamp is also an assignment. You do all your work in your own fork, tag each finished step, and submit it through the form.

> ⛔ **Do not open pull requests to this repository.** Your work stays in your fork.

## 1. Fork the repository

[Step 00](step-00-readiness-check/README.md#part-a-set-up) walks you through sections 1 and 2 click by click. In short: on [panaversity/learn-ai-at-work](https://github.com/panaversity/learn-ai-at-work), click **Fork**, keep your own account as the owner and the name `learn-ai-at-work`, and click **Create fork**.

## 2. Clone your fork

In GitHub Desktop, choose **File → Clone Repository**, pick `<your-username>/learn-ai-at-work`, and click **Clone**. When asked how you plan to use the fork, choose **For my own purposes**. Then set up your Claude project as the README's [How we work](README.md#how-we-work-local-first-human-in-the-loop) describes.

## 3. Keep your fork in sync

Before each step, click **Sync fork → Update branch** on your fork's GitHub page, then **Fetch origin** and **Pull origin** in GitHub Desktop. Don't edit the bootcamp's own files (`README.md`, `AGENTS.md`, `SUBMITTING.md`, each step's `README.md`, or `copperleaf/`), so syncing never conflicts.

## 4. Do the work in each step folder

Save everything you make for a step in its `work/` folder, and write `NOTES.md` in the step folder: what you made, the choices you made, what you checked and how, and how ChatGPT's run compared with Claude's. Deliverables made in the apps (sheets, documents, slides) are exported into `work/` as files.

## 5. Keep real data out

Your fork is public. Use only Copperleaf's fictional files, or made-up (synthetic) material from your own field that you write from scratch ([10.2 Can this data go in, and by which route?](https://agentfactory.panaversity.org/managing-ai-workers/governance-and-responsible-use/can-this-data-go-in/)). Real material with the names changed isn't safe: amounts, dates and other details can still identify people and companies. Never commit passwords, account exports or real customer data. If you commit something real by mistake, tell your instructor and remove it; deleting the commit alone isn't enough, because the history stays public.

## 6. Tag each finished step

Commit the step in GitHub Desktop, then in **History** right-click the commit, choose **Create Tag…**, name it `step-NN-done` (for example `step-01-done`), and click **Push origin**.

**Need to resubmit?** Never move or delete a tag you have already submitted, because the grader may already have read it. Fix the work, commit it, tag the new commit `step-NN-done-v2` (then `-v3`, and so on), push, and submit the new tag through the form.

## 7. Repeat it in ChatGPT

Every step's job is done in Claude and repeated in ChatGPT. Save ChatGPT's result in `work/` too. With only one of the two apps, write a transfer plan in `NOTES.md` instead: the inputs, instructions, permissions and checks the other app would need, marked *planned, not tested*.

## 8. Submit the step

**📝 Submission form: `TODO: FORM LINK (the bootcamp team will add it here)`**

For each step, the form asks for:

| Field | Example |
| --- | --- |
| Your fork's URL | `https://github.com/<your-username>/learn-ai-at-work` |
| Step tag | `step-01-done` |
| Screenshot: Claude | The step's job running or finished in Claude |
| Screenshot: ChatGPT | The same job in ChatGPT (or "transfer plan" if you have one app) |
| Defence video (steps 7, 16, 20, 23 and 24 only) | A link to your recorded project defence |

### Before you share a screenshot or recording

Your screenshots and recordings are public evidence, so check every one before you share it. This is compulsory:

- [ ] **Notifications off.** Turn on Do Not Disturb or Focus, so no message pops up while you record.
- [ ] **Nothing else open.** Close other tabs, windows and apps; record one window if you can.
- [ ] **No account details.** No email addresses, phone numbers or account menus, and no sidebar showing the titles of your other chats.
- [ ] **No secrets.** No passwords, API keys or tokens, and no settings page that shows them.
- [ ] **No unrelated files.** No desktop, downloads folder or file list showing your own files.
- [ ] **No private messages.** No inbox, chat or message history from your other work or life.
- [ ] **Only made-up data.** Copperleaf's files, or material you made up yourself.
- [ ] **Watched back.** Look through it before you share, and crop or record again if anything slipped in.

## 9. How each step is graded

Each step is graded out of 10 and passes at 7. The grader reviews your fork at the step's tag.

| Criterion | Points | What the grader checks |
| --- | --- | --- |
| Done in Claude | 2 | The step's job was done in Claude, as the deliverables and screenshot show. A feature the step asks you to run live (a project, scheduled or triggered task, connector, skill or cloud session) that you could only run by hand, clearly labelled **simulated**, earns 1 |
| Repeated in ChatGPT | 2 | The same job done in ChatGPT and compared with Claude's. A complete transfer plan marked *planned, not tested* earns 1. **A step loses at most 1 point in total for route limits:** if you simulated a feature (above) and also wrote a transfer plan, the transfer plan earns 2, so the step can still reach 9 |
| Makes what the step asks | 2 | Everything in the step's **What you will make** and **Submission checklist** is in `work/` |
| Fit for its reader | 1 | Clear, in the right form, and something Copperleaf's manager could use as it is |
| Checked and governed | 2 | Numbers and claims traced to their sources, the checks done before the work was kept (from step 18, written before the run), no real data, and the worker kept inside its limits |
| NOTES.md | 1 | A short explanation, in your own words, of what you made, what you checked and what you changed, and how many hours the step took you |

**Project defence (steps 7, 16, 20, 23 and 24):** pass or fail. A step that needs one doesn't pass without it.

**Automatic fail for the step:** real personal or company data in your fork or the apps, an invented figure or citation presented as checked, a simulated run or a transfer plan presented as a live one, an action the step said only a person may take (such as sending a message outside Copperleaf), or work copied from another learner.

**Capstone (step 24):** graded on the book's [Part II capstone rubric](https://agentfactory.panaversity.org/managing-ai-workers/overview/#the-part-capstone): six criteria, each Not yet (1), Meets (2) or Exceeds (3); to pass you need at least Meets on every criterion and 14 of 18 points. A review contract written after the run fails the capstone. It also needs its project defence and your PCAO-F sample exam scores in `NOTES.md`, with a screenshot of the results page saved in `work/` as evidence. The capstone is complete only when `NOTES.md` also has the required-reading paragraph: after reading [Sell the work, not the software](https://agentfactory.panaversity.org/from-skills-to-income/sell-the-work-not-the-software/) and the three pages after it, which service you would sell first, to whom, and at what price per result. It earns no points, but a capstone without it is returned as incomplete. For portability, a transfer plan can reach Meets but not Exceeds: Exceeds needs a real run in both apps.

**The changed-data check (compulsory, once, before you graduate).** Your graders keep a changed copy of Copperleaf's files that you have never seen: some amounts, payments and credit limits are different. After you submit the capstone, they send it to you, and within 48 hours you rerun your job on it with the same brief, envelope and review contract, and check the result. Do it in one of two ways: live, on a call with a grader watching, or in one continuous, uncut screen recording (up to ten minutes) that starts with you opening the file they sent. If your capstone used your own role, run your step 20 Copperleaf worker on it instead. It is pass or fail, and you don't graduate without a pass: if you understand the work, the same setup gives the right answer on new data.

## 10. Defend your work

Claude does much of the work, so the bootcamp checks that you understand and own it. At the end of each milestone (steps 7, 16, 20, 23 and 24) you record a **project defence**: a screen recording, with your voice, of you walking through your own work. It is the conversation a manager, a client or an interviewer will have with you.

**Length:** up to five minutes (up to ten for the capstone). **Where:** any link the grader can open without signing in.

**How to record:** your computer can already do it, with your voice. On a Mac, press Shift-Command-5 and choose to record the screen, with your microphone turned on under **Options** ([Take a screenshot or screen recording on Mac](https://support.apple.com/guide/mac-help/take-a-screenshot-or-screen-recording-mh26782/mac), Apple). On Windows, open the Snipping Tool and choose **Record** ([Use Snipping Tool](https://support.microsoft.com/en-us/windows/use-snipping-tool-to-capture-screenshots-00246869-1843-655f-f220-97299b865f6b), Microsoft). Upload the video to any service that gives you a link, such as Google Drive or YouTube (set to *unlisted*), and check the link works in a private browser window before you submit it.

Cover these things, in your own words:

1. **It works.** Show the job running or finished in Claude or ChatGPT, in under a minute.
2. **One claim, end to end.** Pick one number or policy statement in your deliverable and trace it to its source: the input file, the KSoR concept, or a calculation you redo on screen.
3. **One governance decision.** One thing the worker may not do, or one piece of data that stays out, and how you made sure of it.
4. **One change you made.** Something the AI produced that you changed, refused or fixed, and why.
5. **From step 21 on, one prompt you wrote yourself.** Show it, and say what it asks for and why.

Talk, don't read: a script written by an AI and read aloud doesn't count as a defence. Before you share the link, go through the [privacy checklist](#before-you-share-a-screenshot-or-recording).

## Getting help

- Re-read the step's README and the book lessons it links, and ask Claude in a thread of your Claude project to explain what is unclear.
- Ask your instructor or classmates through the bootcamp's usual help channel. Don't use pull requests for questions.
