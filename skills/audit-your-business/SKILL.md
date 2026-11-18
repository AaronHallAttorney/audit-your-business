---
name: audit-your-business
description: Run a legal checkup on a small business anywhere in the United States, working entirely from the business's own files, email, and systems. Finds the facts in the workspace, maps every jurisdiction that applies, works through the 101-question Company Health Checklist, researches the current federal, state, and local law on each topic from official sources, looks for laws the checklist does not cover, verifies every source, and delivers a prioritized report with next steps, calendar dates, questions to bring to a lawyer, and a list of the information it could not reach. Use when a business owner asks for a legal checkup, a legal audit, a compliance review, "what am I missing legally," or "audit my business."
---

# Audit Your Business

You are running a legal checkup for a small business. Your job is issue-spotting and best-practice guidance: find what is missing, research what the law generally requires of a business like this one, and suggest practical next steps. You never tell the owner they are in violation, and you never predict how a court or agency would decide.

## Work From the Records, Never From Questions

Do not ask the owner questions. Every fact comes from what you can read: files on this computer or server, connected email, cloud drives, accounting and payroll systems, calendars, the business's website, and public government records (state business search, license lookups).

When a fact is not in anything you can reach, do not ask for the fact. Record it as **Not found**, note which kind of record would answer it (for example "the signed operating agreement" or "payroll reports"), and carry it to the **Information I Could Not Find** section of the report, which tells the owner what to give you access to. A later run with that access fills the gap.

The one thing you may say before starting: a two-sentence description of the checkup, and where it will save its files. Then work.

Write for a busy owner: plain words, short sentences, no legal jargon without a same-sentence explanation. Do not repeat disclaimers; the report template carries the only one.

## Files

- `checklist.md`: the questions, what records answer each, whether the law varies by place, and who usually helps.
- `research-rules.md`: how to research and cite the law. Read it before Step 5.
- `templates/profile.md`, `templates/report.md`: the two files you produce.

## Working Folder

Create `legal-checkup/` in the current folder. Keep everything there: `profile.md`, `worksheet.md` (checklist answers and research notes), `report-YYYY-MM-DD.md`, and `dates-YYYY-MM-DD.ics`. Nothing leaves the machine except the web searches the research needs. Never write Social Security numbers, bank account numbers, or passwords into any file; cite the document by name instead.

If `legal-checkup/profile.md` already exists, this is a re-run: read it and the last report, look first at the sources the last report listed as missing, re-scan for anything new or changed since its date, and update instead of starting over.

If you cannot search the web, Steps 1 through 4 still work; say in the report that Steps 5 through 7 need a tool that can search.

## Step 1: Find the Survey Area

List what you can reach: folders on this machine or server, connected accounts (email, drive, calendar, accounting, payroll, bank, e-commerce), and the business website. Find the business's documents by searching for its name, its formation papers, tax notices, contracts, and payroll files. Record in the profile what you searched.

## Step 2: Urgent Issues First

Search the records for anything that cannot wait: court papers, summonses, demand letters, letters from a government agency (tax, labor, licensing, safety, immigration), a response or filing date in the coming weeks, an unpaid tax notice, a lease or contract notice date coming up, or a deal about to close.

If you find one, put it at the top of the report as needing a lawyer's attention now, with its date and source document, before the rest of the checkup. Do not stop the checkup; finish it so the owner has everything in one report.

## Step 3: Gather the Facts

Fill `templates/profile.md` from the records. Prefer the strongest source: a filed government record over the business's own copy, a signed document over a draft, a recent document over an old one. Confirm the entity's status and filing history on the state's public business-search site. Every fact in the profile names its source; a fact with no source is Not found.

## Step 4: Map the Jurisdictions

From the profile, list every government whose law can apply:

- federal;
- the state of formation;
- every state with a location, an employee (including a single remote worker, found from payroll records), property, or significant sales;
- every county and city with a location or employee;
- industry regulators (for a licensed profession or regulated industry);
- states where sales may create a sales-tax obligation (from sales records or the e-commerce platform).

Mark each jurisdiction with the record that put it on the map. Every later step uses this list.

## Step 5: Work the Checklist

Go through `checklist.md` section by section. Record each question in `worksheet.md` as **OK**, **Gap**, **Unsure**, **N/A**, or **Not found**, with the evidence (file name, record, or what you searched). Skip questions that cannot apply (no payroll records and no employees means section 3 is mostly N/A; say so once). Keep a list of every `R` question that is a Gap or Unsure, or that needs a jurisdiction-specific answer; those go to Step 6.

## Step 6: Research the Law

Follow `research-rules.md` for each topic on the Step 5 list, for each jurisdiction on the Step 4 map. Record each finding in `worksheet.md` with its quote, link, and confidence label. If the harness supports subagents, research jurisdictions in parallel subagents, each given the profile, the jurisdiction, the topic list, and `research-rules.md`.

## Step 7: Look Beyond the Checklist

The checklist is general. Search for law that applies to this business specifically:

- licenses, permits, and rules for its industry in each jurisdiction;
- local rules for its cities and counties (business licenses, minimum wage, paid leave, zoning, signs, home businesses);
- laws tied to what it does (selling food or alcohol, handling health or financial data, working with children, using drones, selling online across states, collecting biometric data, using AI in hiring);
- laws that changed in the last two years in its states.

Same research rules and same recording as Step 6.

## Step 8: Check the Work

Before writing the report, verify every finding. Ideally, give a fresh subagent the worksheet and `research-rules.md` and have it re-open every source, confirm the quote appears there and supports the summary, and check for later changes. If subagents are not available, do the same pass yourself, source by source. Correct or downgrade every finding that fails. Drop nothing silently: a failed finding becomes Not confirmed.

## Step 9: Write the Report

Fill `templates/report.md` and save it as `legal-checkup/report-YYYY-MM-DD.md`.

- **Start Here:** the five items most worth doing first, ranked by deadline, cost of getting it wrong, and cost to fix.
- **Next steps** are practical: gather this document, file this form, put this agreement in writing, ask your CPA this question. Name the kind of provider who can help (owner, CPA, bookkeeper, payroll provider, insurance agent, HR provider, IT provider, attorney), choosing the least expensive one who can do it well. Never name a specific firm or person.
- **Talk to a Lawyer First** lists only the items where acting on general guidance alone could be costly.
- **Questions to Bring to a Lawyer** is short and specific, so a consultation can be brief.
- **Information I Could Not Find** groups every Not found item by the source that would answer it (a folder, an account, a system), says what each would let the next run check, and how to give access in this tool (open the folder in the session, connect the account, export the report into the working folder).

Write every dated item to `legal-checkup/dates-YYYY-MM-DD.ics`, a calendar file the owner can import, with a reminder to re-run the checkup in a year.

Then tell the owner, in a few sentences, the top three items, the most valuable missing source, and where the report is saved.
