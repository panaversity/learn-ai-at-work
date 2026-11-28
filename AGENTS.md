# AGENTS.md

Guidance for AI agents (Claude, Codex, Cursor and others) working in this repository. Read it before making changes. Where it conflicts with a direct instruction from a maintainer, the maintainer wins.

## What this repo is

**Put AI Workers to Work: The CCAO-F Bootcamp** (repo `learn-ai-at-work`) is a hands-on bootcamp that teaches **knowledge workers** to hand AI whole jobs, check what comes back, and manage an AI Worker, in small, incremental steps. It is a companion to [The AI Agent Factory, Second Edition](https://agentfactory.panaversity.org/) by Panaversity.

- **Name:** call this program a **bootcamp** ("Put AI Workers to Work: The CCAO-F Bootcamp"), not a course, workbook or lab. "Lab" is reserved for the book's in-chapter exercises (for example Lab 5). Use "repo" only for the Git repository itself.
- **Teaching principle: learn by doing.** The book gives the concepts, and the bootcamp is where learners practise them on real knowledge work. Every step must end with something the learner makes, checks and keeps (a sheet, a memo, a brief, a contract, a policy), done in Claude and repeated in ChatGPT. Don't add steps or sections that are only reading or explanation; link the book for theory.
- **Audience: absolute beginners.** This is where a learner's journey starts. Assume no knowledge of AI, Git, GitHub, the terminal or Markdown, only everyday computer use (email, a browser, a spreadsheet). Learners are knowledge workers and other non-developers (accountants, analysts, managers, administrators) preparing for **PCAO-F** (Panaversity Certified Associate: Foundations) and **CCAO-F** (Claude Certified Associate: Foundations). Learners write no code and never use a terminal. Where a step uses a small script (step 7, following the book's Case 4), Claude writes it and the learner checks it by its results, not by reading the code.
- **Place in the family:** this is the first of three bootcamps, and the README's "What comes next" section points learners on. It is followed by [Build and Sell MCP Apps: The CCDV-F Bootcamp Part I](https://github.com/panaversity/learn-mcp) and Build and Sell Self Improving AI Workers: The CCDV-F Bootcamp Part II (under development). Keep building topics (MCP servers, code, connectors you write yourself) out of this bootcamp; they belong to the later ones.
- **Status:** every step is **written in full and in testing** with learners. Each step folder has a complete README; the banner stays until a step has been tested in Claude and ChatGPT.

## The book

- **Scope:** the bootcamp covers the book from its first page to the end of Part II, the PCAO-F syllabus: the opening pages (Preface, The Five Horizons, How to Use This Book, Certification and Portfolio Roadmaps, The FDE 2027 Master Plan, From Skills to Income), **Claude and ChatGPT 2.0** (`/claude-and-chatgpt-2/`, with its reference appendix), **Part 0** (`/how-ai-works/`, chapters 0.1 to 0.4), **Part I** (`/ai-worker-paradigm/`, chapters 1 to 4), **Part II** (`/managing-ai-workers/`, chapters 5 to 11 and the part capstone) and **Appendix C** (`/appendices/exams/associate-foundations/`). `Learn first` links must come from those sections. Never link Part III or later.
- **URLs:** lessons follow `https://agentfactory.panaversity.org/<section>/<chapter>/<lesson>/`, for example `/managing-ai-workers/the-four-part-brief/four-parts/`. The book is updated continuously, so check that every link loads (HTTP 200, not a redirect to another site) whenever you edit a step.
- **Edition:** link only to the current (second) edition at `agentfactory.panaversity.org`. **Never use or link `agentfactory1.panaversity.org`**, the deprecated first edition, or any page that redirects there.
- **Source of truth:** a maintainer's local clone of the book's source is the source of truth for its content. When a step and the book disagree, follow the book and fix the step.

## Target apps

- **Primary:** Claude Desktop (in a Claude project; the Code tab as a fallback) and claude.ai.
- **Must also work in:** the ChatGPT desktop app. Every step's job is repeated in ChatGPT, or, for a learner with only one account, covered by a transfer plan marked *planned, not tested*, as the book allows.
- Teach features both apps share. Where they differ, say so in the step and point to the book's "in your own app" lesson (each chapter's `both-ai-vendors` page).

## How learners work (workflow standard)

The Panaversity AI Method (book: How the Panaversity team works): define the problem, set up the environment, write the four-part brief, improve with the Dr. Gilsdorf method, check and commit. Local first, with a human in the loop. Learners clone their fork with GitHub Desktop, create a Claude project, add the local folder and their GitHub fork to it, and work in the project's threads. Claude reads Copperleaf's files and writes deliverables into the step's `work/` folder, and is told never to commit or push. ChatGPT doesn't work on the folder, so learners attach the files a step needs (or a zip) and save its results into `work/` themselves; learners on a free Claude plan do the same in an ordinary Claude chat until they upgrade (Step 00, A9). The learner checks the work, then commits, tags and pushes in GitHub Desktop. For long-running jobs while their computer is off, they start a cloud session on their fork and review what it brings back. The root README's "How we work" section and `docs/panaversity-ai-method.md` are the learner-facing versions; keep all three in sync, and keep the method page matching the book's How the Panaversity team works page.

## Repository layout

```
.
├── AGENTS.md                 # this file
├── CLAUDE.md                 # imports AGENTS.md, because Claude reads CLAUDE.md
├── README.md                 # bootcamp overview and roadmap
├── SUBMITTING.md             # how learners fork, tag, submit and defend
├── LICENSE                   # MIT
├── .gitignore
├── assets/                   # hero and diagrams: assets/src/*.svg rendered at 2x to light and dark PNGs
├── docs/                     # learner guides: affordable-ai.md, panaversity-ai-method.md (the five-step method mapped to the bootcamp, linked from the README, Step 00 Part A and every step's `## Do it with Claude`), ccao-f-skills-map.md (21 skills → step, evidence, assessment)
├── copperleaf/               # the client's fictional files: customers, invoices, payments, credit policy, emails, archive
└── step-NN-<name>/
    ├── README.md             # bootcamp-owned: plan, prompts, checklist
    ├── work/                 # the learner's deliverables for the step
    └── NOTES.md              # the learner's own write-up
```

### Step folders

- Name them `step-NN-<descriptive-name>`. Never rename an existing step folder without asking, because the README links point to these paths.
- The current steps are:
  0. `step-00-readiness-check` (titled "Step 00: Get Set Up and Check You're Ready"): a guided setup (GitHub account, GitHub Desktop, fork, clone, both AI apps, the Claude project) and how to give ChatGPT the files and work on a free Claude plan, followed by seven short self-checks (the two apps, files and zip files, GitHub Desktop, Markdown, spreadsheets, keeping data safe, working in a Claude project), each with a test that matches its "You're ready if" promise and failures sent to exact book sections. Not graded and not counted in the 24 steps. Keep it short
  1. `step-01-first-whole-job`: The New Way of Working, Tour of the Apps
  2. `step-02-three-deliverables`: Build Something
  3. `step-03-behind-the-screen`: Behind the Screen
  4. `step-04-second-opinion`: Case 1
  5. `step-05-overnight-client-job`: Case 2
  6. `step-06-shared-worker`: Case 3
  7. `step-07-month-end-setup`: Case 4
  8. `step-08-the-big-picture`: The Five Horizons, the Preface, How to Use This Book, the Certification and Portfolio Roadmaps, The FDE 2027 Master Plan and From Skills to Income (every opening page, in book order)
  9. `step-09-what-ai-actually-is`: chapter 0.1
  10. `step-10-markdown`: chapter 0.2
  11. `step-11-ai-fluency`: chapter 0.3
  12. `step-12-critical-thinking`: chapter 0.4, then the Basic Concepts sample exam
  13. `step-13-chatbots-to-ai-workers`: chapter 1
  14. `step-14-role-contract`: chapter 2
  15. `step-15-operating-rhythm`: chapter 3
  16. `step-16-architecture`: chapter 4
  17. `step-17-four-part-brief`: chapter 5
  18. `step-18-review-contract`: chapter 6
  19. `step-19-authority-envelope`: chapter 7
  20. `step-20-knowledge-and-state`: chapter 8
  21. `step-21-recurring-work`: chapter 9
  22. `step-22-governance`: chapter 10
  23. `step-23-when-it-goes-wrong`: chapter 11
  24. `step-24-capstone`: the Part II capstone, then the PCAO-F sample exam
- **Book order and coverage.** The steps follow the book's own order, one book section per step, and every page PCAO-F tests has a step: Claude and ChatGPT 2.0 (steps 1 to 7, one per case from step 4), the opening pages, from The Five Horizons to From Skills to Income (step 8), Part 0 (steps 9 to 12, one per chapter), Part I (steps 13 to 16), Part II (steps 17 to 23) and its capstone (step 24). Claude and ChatGPT 2.0, The Five Horizons, the Preface and Part 0 are what PCAO-F's Basic Concepts exam tests (steps 1 to 12). Every practice task in section 6 of Anthropic's CCAO-F exam guide, version 1.1, has a step (see the README's CCAO-F map); keep that table in sync. Estimated time is 130 to 170 hours; re-estimate when a step's work changes. The step count follows the material, not the other bootcamps: split a step that crams too much for a beginner.
- **Living documents carry forward.** From step 14, the Role Contract (and later the brief, review contract, Authority Envelope, KSoR and Governance Record) grows step by step. Each step's first prompt copies the previous step's `work/` living documents into the new step's `work/`, so every step folder stands on its own and earlier steps stay as they were graded.
- Prompts must never ask Claude to edit a step's `README.md` or Copperleaf's client files. Learner write-ups go in `NOTES.md`.

## The client: Copperleaf Supply

Every step is framed as work for one fictional client, **Copperleaf Supply**, a family-owned distributor of coffee, cups, cleaning and kitchen supplies to about 600 cafés, restaurants and hotels, with 45 staff. The learner joins its finance team as the person who puts AI to work. Its people: **Amira** (owner), **Rosa** (finance manager, accountable owner of the Receivables Worker and approver of its knowledge) and **Ben** (credit controller).

- The running example is accounts receivable: matching payments, aged-debt reporting, reminders, credit holds, disputes and write-offs. From step 14 it becomes one AI Worker, the **Receivables Worker**. The book's own example is Brightline's accounts-payable Worker; keep Copperleaf on the receivables side so learners transfer the book's ideas instead of copying its labs.
- Copperleaf's files live in `copperleaf/` (see its README). Its world is set on Monday 2 November 2026. The files are generated to contain deliberate problems for the steps to find (partial, over-, duplicate, already-paid, combined, unreferenced and unmatched payments in `payments-week-44.csv`; a disputed invoice; Harbourline's invoices more than 70 days overdue; Station Square's 85-day-old invoice, paid only last week; a fraudulent refund email with an embedded instruction to "any AI assistant"; a superseded credit-limit sheet in `archive/` that wrongly puts The Lantern Room over its limit). Step 23 also has a bootcamp-owned `failed-run/` folder (the brief, task record and output of a run that used the archive sheet and the old 45-day terms), which learners read but don't change, and step 21 has the learner create one inbox file, `work/inbox/payments-2026-11-03.csv`, from text given in the step. Keep test answers in step READMEs consistent with these files, and keep the answer key for graders out of the repo (it lives in the project's shared files, as `answer-key-graders.md`, with a changed copy of the client files for the capstone's changed-data check in `grader-variant/`). **Never give answers away inside the client files:** no notes saying which file is stale or which email is fraud, because the AI reads those files too and the test becomes trivial.
- Copperleaf's five KSoR concepts (step 20) are payment terms, credit limits and holds, the reminder schedule, disputes and credit notes, and write-off approval.
- Each step README has a one- or two-sentence `> 🍃 **Copperleaf's ask:**` blockquote right after the summary. Keep it a light touch, and consistent with the root README's "Your client" section.
- Learners may use a real task from their own role instead (always allowed in the capstone), but only rebuilt with made-up (synthetic) data, as book lesson 10.2 supports; real data with the names changed isn't allowed.
- Copperleaf may later appear as one of Stockroom's customers in the CCDV-F bootcamp. Keep the two consistent if either changes.

## Checking and governance

Checking is this bootcamp's first-class theme, as multi-tenancy is in the CCDV-F bootcamp. Keep these rules in every step:

- **Nothing is used unchecked.** Every deliverable is checked before it is kept: numbers re-done, policy claims traced to the handbook or the KSoR, facts traced to the inputs, assumptions labelled.
- **Checks come first.** From step 18, the review contract is committed before the run, so its date in the learner's history comes first.
- **A person signs.** Nothing goes to a customer, the bank or anyone outside Copperleaf without the accountable person's sign-off. No step ever sends a real email or message.
- **Data care.** Learners' forks are public. Only the bootcamp's fictional files, or synthetic material the learner makes up from scratch, ever go into the apps or the repo.
- **Proof.** Every step's submission checklist has a `Checked:` item, and the rubric fails any deliverable that presents an invented figure or citation as checked.

## Writing step READMEs

Every step follows this structure:

1. `# Step NN: <Title>`
2. Status banner `> 🚧 **Under development.** …` (remove it only when the step has been tested with learners in Claude and ChatGPT)
3. One-paragraph summary
4. `> 🍃 **Copperleaf's ask:** …`, then `> ⏱️ **About N to M hours** …` with good places to pause (instruction numbers). Keep the per-step hours adding up to each milestone's range in the README. Below it, where they apply: `> 🆓 **On the free route:** …` (how to simulate a paid feature, labelled *simulated*; steps 3, 5, 6, 7, 13, 19, 20, 21, 24) and `> 🧭 **Your prompts in this step:** …` (Modify in steps 13 to 20, Construct in 21 to 23, On your own in 24)
5. `## Learn first`: book lessons, each with a one-line reason, ending with the section's `check-yourself` page where the book has one. The book's lab is linked as "the book's version of this step": the Copperleaf job replaces it, and doing both is optional extra practice
6. `## Why this step matters`
7. `## What you will learn`
8. `## What you will make`
9. `## Key concepts` (bold term, then a one-sentence definition, in the book's words)
10. `## Do it with Claude`: a one-line `> 🛠️` note linking `docs/panaversity-ai-method.md` (not the `> 🧭` prompt-level note), then numbered instructions, each with a copy-paste prompt in a ```` ```text ```` block
11. `## Repeat it in ChatGPT`: what to carry over, and the transfer-plan fallback
12. `## Check it`: the checks the learner runs before keeping the work
13. `## Record your defence` (defence steps only: 7, 16, 20, 23 and 24)
14. `## Keep it`: always the last thing the learner does, after the ChatGPT part, notes and defence: four numbered GitHub Desktop actions (read **Changes**, commit with the step's summary, **Create Tag…** `step-NN-done`, **Push origin**). Commits that must come before a run (review contracts, plans, checks) stay in the instruction where they happen
15. `## Submission checklist`, with a **Checked:** item naming what the learner verified themselves
16. `## References`
17. Footer navigation: previous step · Roadmap · next step

Step 00 is the exception: banner, summary, Copperleaf's ask, `## How it works` (a short numbered order of work and a check → book → time table), `## Part A: Set up` (click-by-click setup, including GitHub), `## Part B: The seven checks` (each with "You're ready if", a test with its answer in a collapsed block, "If not, read" book sections, and "Outside the book" links only where the book has no coverage), `## Part C: Save your results`, `## Finding things in the apps` (a reference of click paths in both apps that later steps link to by anchor when a feature is first used: threads and naming, ordinary and incognito chats, ask-before-acting, models, web search, memory, skills and connectors, scheduled tasks, and a cloud session with reviewing and merging its branch), `## What you will make`, `## Submission checklist` and the footer.

Style:

- Plain, friendly, encouraging English in full sentences, for absolute beginners. Explain any term the first time it appears, in the book's words, and add new everyday terms to the README's "Words you will meet" table.
- Give click-by-click instructions (which app, which menu, which button), one action per numbered line, and say what the learner should see when it worked.
- Never assume a terminal, a command or a code editor.
- Describe actions in the apps generically where menus may change, and give each app's name for a feature only when the book does.
- Prompts are written as the learner would type them, are self-contained, and ask Claude to plan before a big job. They end with the learner checking the work and committing in GitHub Desktop.
- Every prompt the learner pastes goes in a ```` ```text ```` block, never inline; only short one-line questions may stay inline.
- **The Dr. Gilsdorf method** (step 4 of the Panaversity AI Method, named by Zia Khan after Dr. Gilsdorf, a business communication professor at Arizona State University): improve work in many small rounds toward 9.5, each with the step's pass-or-fail checks, an AI review and a grade out of 10, then a different AI's independent review (made without the first AI's grades) pasted back and the checks run again. A failed check always outweighs a grade. Introduced hands-on in step 2 (instruction 6a), done in full in step 4, and described in the README's "How we work". Don't add biographical details about Dr. Gilsdorf beyond these. Always pair it with: a grade is an opinion, check the facts, and share content across AI providers only when allowed.
- **Prompts fade on purpose.** Steps 1 to 12 give every prompt (Follow). Steps 13 to 20 give prompts the learner adapts and records one change (Modify). Steps 21 to 23 give each prompt's goal and how to tell it worked (never the example's content), with the example folded in a `<details>` block (Construct); the copy-forward prompt in instruction 1 stays visible. Step 24 gives only tasks and checks (On your own). Keep this when editing or adding prompts.
- **Free and professional routes.** The README's "What it costs: two routes" is the single source. A feature a learner can only simulate is labelled *simulated* and, like a transfer plan, earns fewer points (SUBMITTING section 9); never write a step that needs a paid plan with no simulated fallback. The README's "What counts as evidence on each route" table is the rule for evidence. A step loses at most 1 point in total for route limits (a simulated feature plus a transfer plan still reaches 9). Every "In your ChatGPT project" instruction carries a no-project fallback (a new chat with the same files attached). The capstone uses only its 18-point rubric (a transfer plan reaches Meets, not Exceeds), and its changed-data check is compulsory once before graduation, supervised or in one continuous recording within 48 hours.
- **Instruction, permission, verification.** Step 3 teaches the three layers; steps 6 and 19 and Step 00 A7 refer back to them. Don't present an instruction to the AI as if it were a lock.
- **Diagrams.** Ten diagrams explain the ideas that are hardest to follow in text: how we work and the bootcamp path (README), the Panaversity AI Method (`docs/panaversity-ai-method.md`), the Step 00 setup map and the three layers (Step 00 and step 03), the life of an invoice (`copperleaf/README.md`), the Dr. Gilsdorf method (step 02), the Four-Part Brief (17), the order of a delegated job (18 and 24) and the Authority Envelope (19). Each has a light and a dark PNG in `assets/`, rendered at 2x from its SVG in `assets/src/`, and is embedded with a `<picture>` element whose alt text describes the whole diagram. When a step changes what a diagram shows, edit the SVG and re-render both PNGs. Diagrams never give away an answer (no Copperleaf figures, traps or test results).
- Optional `> 🌍 **Optional: in your own field.**` exercises (steps 1, 7, 12, 18, 22) use material the learner makes up from scratch, never real data (renaming people in real material isn't enough). Every defence section links SUBMITTING's privacy checklist for screenshots and recordings. Copperleaf stays the one running project.
- When a step uses an app feature, link the matching section of Step 00's "Finding things in the apps" rather than repeating the click path.
- Accounting words are defined once, in `copperleaf/README.md` ("Receivables in five minutes"); link there rather than redefining them.
- Learners who use only ChatGPT use `work/chatgpt/` wherever a step names a `work/claude/` file (the README and step 02 say so); keep paths consistent with that.
- Git work is GitHub Desktop actions (Changes, Commit, History → Create Tag…, Push origin), never terminal commands.
- When a step's status changes, update the step's banner and the **Status** column of the roadmap in `README.md`.

## Keeping things in sync

When you add, rename or reorder a step, update together: the step folder name, the roadmap table, the milestones table and the CCAO-F map in `README.md`, the previous/next links in the neighbouring steps, the step list in this file, the defence steps in `SUBMITTING.md`, and the step count badge in `assets/src/hero-light.svg` and `assets/src/hero-dark.svg` (then re-render both PNGs at 2560×1280).

Keep the "How we work" section of `README.md`, Step 00's Part A, and the "How learners work" section above saying the same thing. Keep `docs/affordable-ai.md` and the README's "What it costs" consistent.

## Students and submissions

This repo is a student assignment. Learners **fork** it, work in their fork, and submit through a form (see `SUBMITTING.md`).

- **Never open pull requests to `panaversity/learn-ai-at-work` on a learner's behalf**, and never suggest it.
- When helping a learner in their fork, don't commit or push: they review, commit and push in GitHub Desktop. Only if they explicitly ask, push to their fork's `origin`, never anywhere else.
- Each finished step is tagged `step-NN-done` and pushed to the fork.
- Learners don't edit bootcamp-owned files (`README.md`, `AGENTS.md`, `SUBMITTING.md`, step `README.md` files, `copperleaf/`), because that causes conflicts when they sync. Their work goes in `work/` and `NOTES.md`.
- At the end of milestones 1, 3, 4, 5 and 6 (steps 7, 16, 20, 23 and 24) learners record a **project defence** (`SUBMITTING.md` section 10). If milestones change, update `SUBMITTING.md`, the root README and the affected checklists together.
- Grading follows the rubric in `SUBMITTING.md` section 9; the capstone also uses the book's Part II capstone rubric. Keep the form link a clearly marked placeholder until the maintainer supplies it.

## Git

- Small, focused commits with descriptive messages, for example `step-17: tighten the Four-Part Brief prompts`.
- Never commit real personal or company data, credentials or exported account data.
- Don't rewrite published history.
