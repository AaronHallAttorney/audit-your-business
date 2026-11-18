# Audit Your Business

A legal checkup for small businesses that runs in your AI assistant: Claude, Codex, or any agent that can read files and search the web.

It works through the **Company Health Checklist**, 101 questions on the legal problems that most often hurt small businesses, written by Minnesota business attorney [Aaron Hall](https://aaronhall.com/audit/). Your assistant then researches the current federal, state, county, and city law for wherever your business operates, so it works for a business in any town in the United States.

## What It Does

It works from your records, not a questionnaire. Your assistant reads the files, email, and systems you give it access to, plus public government records, and never asks you to fill anything in.

1. **Surveys what it can reach:** folders on your computer or server, connected email, drives, accounting and payroll systems, and your website.
2. **Looks for anything urgent first:** court papers, agency letters, response deadlines, notices about to run out.
3. **Gathers the facts** about your business from those records, citing the document behind each one.
4. **Maps every jurisdiction that applies:** your formation state, every state where you have a location or an employee (even one remote worker), your cities and counties, and your industry's regulators.
5. **Works the checklist:** entity records, taxes, workers, contracts, real estate, intellectual property, data and privacy, insurance, and your advisor team.
6. **Researches the law** on each topic from official government sources, quoting each source and labeling how confident it is.
7. **Looks beyond the checklist** for laws specific to your industry, locations, and activities, and for recent changes.
8. **Checks its own work:** a second pass re-opens every source and confirms it says what the finding claims.
9. **Writes a report:** the five things to do first, dates for your calendar (also as a file you can import), every finding with its source, who can help with each item (often not a lawyer), questions to bring to a lawyer, and a list of the records it could not reach.

The more it can read, the more it can check. The report's **Information I Could Not Find** section tells you exactly which folders or accounts to give it next. Everything stays in a `legal-checkup/` folder on your computer. Run it again after granting access, in a year, or when something changes, and it picks up where it left off.

## Install

**Claude Code**

```
/plugin marketplace add AaronHallAttorney/audit-your-business
/plugin install audit-your-business@audit-your-business
```

**Claude apps (claude.ai, desktop):** zip the `skills/audit-your-business` folder and upload it as a skill under your Claude settings. Code execution and web search should be on.

**Codex:** copy `skills/audit-your-business` into `~/.agents/skills/`.

**Any other agent:** open this folder in your agent and ask it to follow `AGENTS.md`.

## Run It

Start your assistant in a folder that holds your business records (or connect the accounts where they live), then ask: *"Audit my business."* A simple business takes well under an hour; a business with several locations takes longer, mostly in research.

## Good to Know

- The research is only as good as the sources your assistant can reach. Each finding is labeled **Confirmed**, **Secondary only**, or **Not confirmed**, so you can see which ones to double-check.
- Some steps are expensive to get wrong (firing someone, reclassifying workers, signing a major contract, answering an agency). The report marks those so you can get help first.

## About

Aaron Hall is a business attorney in Minneapolis, Minnesota. The original checklist has helped business owners since 2014: [aaronhall.com/audit](https://aaronhall.com/audit/).

## License

[CC BY 4.0](LICENSE). Share and adapt it freely, including commercially. Required credit: "[Company Health Checklist](https://aaronhall.com/audit/) by Aaron Hall," with the link to https://aaronhall.com/audit/ wherever a link is possible (on the web, a live hyperlink).

General information, not legal advice.
