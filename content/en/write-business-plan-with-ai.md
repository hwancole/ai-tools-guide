---
title: "How to Write a Business Plan with AI (Step by Step)"
description: "Use ChatGPT, Claude, Gemini or Copilot to draft a business plan: section-by-section prompts, a lean one-page option, financials you can check, and what AI gets wrong."
date: 2026-11-11
key: write-business-plan-with-ai
tags: [small-business, prompts, chatgpt, claude, gemini, copilot, work]
cover: /images/write-business-plan-with-ai.svg
coverAlt: "A document titled Business Plan with section lines and a rising bar chart, next to a chat bubble"
---

AI chatbots can turn your notes into a well-structured business plan draft in an afternoon. They are good at structure, wording and asking you the questions you forgot. They are bad at knowing your real costs, your local market and the numbers a lender will check. The method below keeps you in charge of the facts and lets the AI do the writing.

> **Quick answer (as of November 2026):**
> 1. Decide the format: a **traditional plan** (several sections, what lenders and investors usually ask for) or a **one-page lean plan** (faster, good for testing an idea).
> 2. Give the AI a **business brief** with your idea, customers, prices, costs and goals, and ask it to **interview you** for missing details (prompt below).
> 3. Draft **one section at a time** using the standard outline: executive summary, company description, market analysis, organization, products, marketing and sales, funding request, financial projections.
> 4. Build the **financial projections in a spreadsheet** from your own numbers. Use the AI to explain and check formulas, not to invent figures.
> 5. Ask the AI to **review the plan like a skeptical lender**, then fix the gaps yourself. Write the executive summary last.

## Traditional plan or lean plan?

The U.S. Small Business Administration (SBA) describes two common formats. Pick one before you start prompting, because the AI will write very different things.

| | Traditional business plan | Lean startup plan |
|---|---|---|
| Length | Can be dozens of pages | Typically one page |
| Time to make | Usually much longer | SBA says it can take as little as an hour |
| Best for | Bank loans, investors, detailed planning | Testing an idea, simple businesses, plans you'll change often |
| Sections | Executive summary, company description, market analysis, organization and management, service or product line, marketing and sales, funding request, financial projections | Key partnerships, key activities, key resources, value proposition, customer relationships, customer segments, channels, cost structure, revenue streams |

*Section lists from the SBA's "Write your business plan" guide (see Sources). If you're applying for a loan or grant, use the lender's or program's own template if it has one.*

## Which AI tool to use

Any of the big assistants can write a plan. The differences are in research and file handling.

| Tool | Free version | Useful for business plans | Things to know |
|---|---|---|---|
| **ChatGPT** | Yes | Web search, limited file uploads and limited deep research on the free plan; data analysis for spreadsheets | Interactive tables and charts are on paid plans; Plus and Pro include full deep research |
| **Claude** | Yes | Web search and file creation (for example a formatted document or spreadsheet) on the free plan | The Research feature starts at Pro ($20/month billed monthly, or $17/month billed yearly) |
| **Gemini** | Yes | Deep Research is listed in the free plan, useful for a first pass at market research | Paid Google AI plans (Plus $4.99, Pro $19.99 a month in the US) raise limits |
| **Microsoft Copilot** | Yes (limited) | Handy if you write in Word and Excel; Copilot in the Office apps comes with paid Microsoft 365 plans | Microsoft 365 Personal is $9.99/month in the US; check the plan page for which apps include Copilot |

*Plan details and US prices as of November 2026, from each vendor's pricing page (see Sources). They change often, and prices differ by country.*

A practical setup: use the chatbot you already like for writing, and a tool with web research (deep research in ChatGPT or Gemini, Research in paid Claude) for the market section.

## Step 1: Write a business brief and let the AI interview you

Generic plans come from generic prompts. Put what you know in one message, then make the AI ask questions.

**Copy-paste prompt: the brief**

```text
I'm writing a [traditional / one-page lean] business plan. Act as an experienced small-business advisor.
Before writing anything, ask me up to 10 questions, one group at a time, about anything important that's missing.

- Business idea: [what you sell, in one or two sentences]
- Location and how you sell: [city/region; online, storefront, mobile, B2B]
- Target customers: [who they are, what problem you solve]
- Prices: [your planned prices]
- Main costs: [rent, equipment, materials, software, staff, etc., with amounts if you know them]
- Competitors I know of: [names or types]
- Stage: [idea / started / running for X months], current revenue if any: [amount]
- Purpose of the plan: [bank loan of $X / investor pitch / grant / my own planning]
- My background: [relevant experience, skills, team]
```

Answer honestly, including "I don't know yet." The AI should mark those points as open questions in the plan instead of inventing answers.

## Step 2: Get an outline that fits your purpose

```text
Based on my answers, create an outline for the plan using these sections: [paste the traditional or lean list].
For each section, list the 3–5 points it should cover for my business and mark which facts I still need to provide with [NEED].
Keep it tailored to a [loan application / investor pitch / internal plan].
```

The [NEED] markers become your to-do list. Fill them before drafting, or the AI will fill them with guesses.

## Step 3: Draft one section at a time

Long one-shot answers get vague. Ask for one section per message and give it the facts for that section.

**Copy-paste prompt: a section**

```text
Write the [Company description] section of my business plan in about [300] words.
Use only the facts below and my earlier answers. Don't invent numbers, customers, partners or awards.
If a fact is missing, write [NEED: ...] instead of guessing.
Tone: clear, plain English, confident but not salesy.

Facts: [paste notes]
```

Tips for specific sections:

- **Market analysis.** Use a web research mode and ask for sources: "Find the size and growth of the [industry] market in [region], plus the main customer trends. Give a link for every number and say how recent it is." Open the links. Prefer government statistics, industry associations and your own local research (competitor visits, price checks, customer conversations) over blog posts.
- **Organization and management.** Paste your real roles and experience. Ask it to present the team's strengths without exaggerating.
- **Marketing and sales.** Ask for a plan with channels, a monthly budget you set, and how you'll measure results: "Suggest 4 low-budget marketing channels for [business] in [city] with a 3-month action plan and one metric per channel."
- **Funding request.** State the exact amount, what it pays for and over what period. The AI can turn your list into a clear "use of funds" table.

## Step 4: Build the financials yourself (with AI as a helper)

Financial projections are where AI does the most damage if you let it guess. A lender will ask where every number comes from.

1. Start a spreadsheet with three tabs: **assumptions**, **monthly forecast (12 months)**, **yearly summary (3 years)**.
2. Put your real inputs in the assumptions tab: prices, expected sales per month, cost per unit, rent, wages, loan payments.
3. Ask the AI to help with structure and formulas, not values:

```text
I'm building a 12-month cash flow forecast in [Excel / Google Sheets].
Assumptions are in a sheet called "Assumptions": price per unit in B2, cost per unit in B3, monthly fixed costs in B4, and expected units sold for months 1-12 in B6:B17.
Write the formulas for monthly revenue, cost of goods sold, gross profit, operating expenses, net profit and ending cash balance.
Explain each formula in one line.
```

4. Ask for a **break-even calculation** from your numbers: "With fixed costs of $X a month, a price of $Y and a variable cost of $Z per unit, how many units do I need to sell to break even? Show the math."
5. Ask for **best, expected and worst case** versions by changing two or three assumptions, so the plan shows you've thought about risk.

For more help with formulas, see our guide to [Excel formulas with AI](https://hwancole.github.io/ai-tools-guide/en/ai-excel-formulas/).

## Step 5: Have the AI review it like a lender or investor

Once all sections exist, paste the full draft (or upload the file) and ask for criticism.

**Copy-paste prompt: the tough review**

```text
Review this business plan as a skeptical bank loan officer [or: early-stage investor].
List:
1. The 10 biggest weaknesses or unanswered questions, most serious first.
2. Any numbers that look unrealistic or inconsistent between sections.
3. Claims that need evidence.
4. Anything missing that a [lender / investor] would expect.
Don't rewrite the plan; just give the list.
```

Fix the issues yourself, then ask for a final pass on clarity and length.

## Step 6: Write the executive summary last

The executive summary is the first page people read, so write it when everything else is final.

```text
Write a one-page executive summary of the plan below. Include: what the business does, the customer problem,
the market opportunity, what makes us different, the team, key financial figures (from the plan only), and the funding request.
Maximum 350 words.
```

Read it out loud. If a sentence sounds like it could describe any business, replace it with a specific fact.

## What AI gets wrong in business plans

- **Made-up statistics.** Market sizes and growth rates without a source, or with a source that doesn't say that. Check every number.
- **Optimistic financials.** Hockey-stick growth with no explanation. Base sales on what you can actually reach: foot traffic, website visits, sales calls.
- **Generic competitor lists.** It may name big brands and miss the shop down the street. Do your own local research.
- **Legal and tax details.** Licenses, permits, business structure and taxes depend on where you are. Check official government sites or a local advisor.
- **Same-sounding text.** Lenders read many plans. Add your real story, real numbers and real customer feedback.

Also be careful with what you paste in. Business plans contain sensitive data like revenue, salaries and customer names. Check your chatbot's privacy settings first; see [how to stop AI training on your chats](https://hwancole.github.io/ai-tools-guide/en/stop-ai-training-on-your-chats/).

## FAQ

**Can AI write a business plan for me?**
It can write a solid draft of every section if you give it real facts. You still need to supply the numbers, check the research and make sure the plan reflects what you'll actually do.

**Which AI is best for writing a business plan?**
For drafting, ChatGPT, Claude, Gemini and Copilot are all capable. For market research, a tool with a web research mode helps: as of November 2026, ChatGPT's free plan includes limited deep research, Gemini lists Deep Research in its free plan, and Claude's Research needs a paid plan. If you work in Word and Excel, Copilot fits into those apps on paid Microsoft 365 plans.

**Is it free to write a business plan with AI?**
Yes. The free versions of all four can draft sections, outlines and reviews. Paid plans mostly add higher limits and more research.

**Will a bank accept a business plan written with AI?**
Banks judge the content: realistic numbers, evidence and a clear repayment plan. Nothing stops you from using AI to help write it, but you're responsible for every claim. Use the lender's own template or checklist if it provides one.

**How long should a business plan be?**
A lean plan is about one page. A traditional plan can run to dozens of pages, but shorter and clearer is usually better. Check what your lender, investor or grant program asks for.

**Can AI make the financial projections?**
It can build the structure, write the spreadsheet formulas and explain the results. The inputs (prices, sales volumes, costs) should come from you and your research, not from the AI.

## Sources

- [U.S. Small Business Administration: Write your business plan](https://www.sba.gov/business-guide/plan-your-business/write-your-business-plan)
- [OpenAI: ChatGPT plans and pricing](https://chatgpt.com/pricing/)
- [Anthropic: Claude plans and pricing](https://claude.com/pricing)
- [Google: Google AI plans (Gemini subscriptions)](https://gemini.google/subscriptions/)
- [Microsoft: Copilot pricing plans for individuals](https://www.microsoft.com/en-us/microsoft-365-copilot/pricing/individuals)
