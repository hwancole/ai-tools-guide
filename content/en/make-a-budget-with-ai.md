---
title: "How to Make a Budget with AI (ChatGPT, Claude, Gemini)"
description: "Use ChatGPT, Claude or Gemini to build a monthly budget from your bank statement: what to share, copy-paste prompts, a sample budget, and how to check the math."
date: 2026-11-17
key: budget-with-ai
tags: [personal-finance, budgeting, spreadsheets, chatgpt, claude, gemini, beginner]
cover: /images/make-a-budget-with-ai.svg
coverAlt: "A list of bank transactions being sorted into a simple monthly budget with category bars"
---

An AI chatbot is good at the boring part of budgeting: sorting a month of transactions into categories, adding them up, spotting subscriptions you forgot about, and turning all of it into a plan you can keep in a spreadsheet. It is not good at knowing your goals, and it can get arithmetic wrong, so you stay in charge of the numbers that matter.

> **Quick answer (as of November 2026):** Download last month's transactions from your bank as a CSV file. Delete account numbers and anything you don't want to share. Upload the file to ChatGPT, Claude or Gemini (free plans accept file uploads, with daily limits) and ask it to group your spending into categories, total each one, and draft a budget that fits your take-home pay and one savings goal. Then copy the result into a spreadsheet and check the totals against your statement before you rely on them.

## What AI can and can't do for your budget

| Good at | Not good at |
|---|---|
| Categorizing a long list of transactions in seconds | Knowing which spending matters to you |
| Finding recurring charges and subscriptions | Exact arithmetic on hundreds of rows, unless it runs code to calculate |
| Suggesting a starting split (for example 50/30/20) | Personalized tax, debt or investment advice |
| Writing spreadsheet formulas and templates | Remembering last month's numbers unless you give them again |
| Explaining budgeting methods in plain language | Seeing your bank account (unless you connect it, see below) |

Treat the AI like a fast assistant who has never met you. It does the sorting and drafting; you decide the targets.

## Step 1: Get your transactions out of the bank

Most banks and card issuers let you download transactions from the website or app, usually under **Statements**, **Activity** or **Export**. Pick **CSV** if it's offered, because a spreadsheet file is far easier for an AI to read than a PDF statement. One full month is enough to start; three months gives a more honest picture, since bills like insurance or car registration don't hit every month.

No export option? You can type a rough list yourself ("rent 1,400, groceries about 450, phone 65...") or paste lines copied from the statement. A budget built from estimates is still better than no budget.

## Step 2: Remove what the AI doesn't need

Before uploading, open the file and delete:

- Full account and card numbers
- Your name and address, if the export includes them
- Transfers between your own accounts (they double-count spending)
- Anything you simply don't want stored in a chat history

The AI only needs **date, description and amount**. If you'd rather not share real merchant names, you can replace them with categories you choose before uploading.

By default, consumer chatbots may use conversations to improve their models, and each has a setting to turn that off. Our guide on [how to stop AI training on your chats](https://hwancole.github.io/ai-tools-guide/en/stop-ai-training-on-your-chats/) walks through the settings in ChatGPT, Claude, Gemini and Copilot.

## Step 3: Upload and categorize

All three major chatbots accept spreadsheet uploads, but limits differ and change often. As of November 2026, from each company's help pages:

| Chatbot | Spreadsheet uploads | Notes |
|---|---|---|
| **ChatGPT** | CSV and other spreadsheet formats | OpenAI says CSV or spreadsheet files can be up to roughly 50 MB depending on row size; free accounts get a small daily upload allowance |
| **Claude** | CSV and XLSX | Up to 20 files per chat, 500 MB each; XLSX needs the code execution and file creation setting turned on |
| **Gemini** | Spreadsheets and most file types | Up to 10 files per prompt, 100 MB each (subject to availability); free accounts have standard usage limits |

A bank CSV for one month is tiny, so you won't hit size limits. If an upload fails, paste the rows directly into the chat instead.

Then use the first prompt below.

## Copy-paste prompts

**1. Categorize a month of spending**

> I've uploaded my bank transactions for [month]. Columns are date, description and amount; negative numbers are spending. Group every transaction into these categories: housing, utilities, groceries, eating out, transport, insurance, subscriptions, shopping, health, debt payments, savings, other. Show a table with the total and percentage of spending for each category, and list any transaction you weren't sure how to categorize so I can decide. Use code to calculate the totals.

**2. Find subscriptions and recurring charges**

> From the same transactions, list every charge that looks recurring (same merchant, similar amount, regular dates). For each, show the amount, how often it appears, and the yearly cost. Mark any that look like duplicates or free trials that turned into paid plans.

**3. Draft a budget**

> My take-home pay is [amount] per month. My fixed bills are [list]. My goal is to [save X per month / pay off a card of X / build an emergency fund of X by date]. Using my actual spending from the table above, draft a monthly budget with a target for each category. Show where I'd need to cut compared with last month, and keep the cuts realistic, not extreme.

**4. Try a budgeting method**

> Explain the 50/30/20 rule and zero-based budgeting in a few sentences each. Then apply both to my numbers and show me the two budgets side by side, so I can pick one.

**5. Turn it into a spreadsheet**

> Create a budget template for [Excel / Google Sheets] with columns for category, budgeted amount, actual amount and difference. Include formulas for the difference column and a total row, and a cell that shows how much of my income is left unassigned. Tell me exactly which cells to put the formulas in.

**6. Monthly check-in**

> Here is my budget from last month and this month's transactions. Compare actual spending with each target, tell me which three categories went over and by how much, and suggest one specific change for next month.

## Example: a simple budget from one month

Say your take-home pay is $4,000 a month and you ask for a 50/30/20 budget. The AI might return something like this:

| Category | Last month | Suggested budget |
|---|---|---|
| Rent and utilities | $1,550 | $1,550 |
| Groceries | $520 | $450 |
| Transport | $230 | $230 |
| Insurance and phone | $170 | $170 |
| **Needs subtotal** | **$2,470** | **$2,400** |
| Eating out | $410 | $250 |
| Subscriptions | $95 | $55 |
| Shopping and fun | $520 | $495 |
| **Wants subtotal** | **$1,025** | **$800** |
| **Savings and extra debt payments** | **$505** | **$800** |

This is an illustration, not advice. The useful part is the shape: the AI shows where last month went and proposes a gap-closing plan you can accept, edit or reject line by line. Notice that needs come to 60% of pay here, well over the 50% guideline, because rent can't shrink overnight. The plan reaches the 20% savings target by trimming wants instead. A good answer will point out a mismatch like this rather than force the numbers to fit the rule.

## Can ChatGPT connect to my bank account?

In the United States, yes. OpenAI launched a **Finances** feature in ChatGPT in May 2026 as a preview for Pro users. It connects to banks, cards and investment accounts through Plaid and shows a dashboard of spending, subscriptions and upcoming payments that you can ask questions about. OpenAI says ChatGPT can see balances and transactions but "cannot see full account numbers or make any changes to your accounts," and that synced data is deleted within 30 days if you disconnect (under **Settings > Apps > Finances**). OpenAI said it would widen access over time, and news reports in November 2026 describe it as open to eligible US users on all personal plans. If you're in the US, look for **Finances** in the ChatGPT sidebar.

Outside the US, or if you'd rather not link accounts, the CSV method above works with any chatbot and keeps you in control of exactly what you share.

## How to check the AI's numbers

AI tools can misread a row or make an addition error, especially on long lists. Before you trust a budget:

- **Check one total against your statement.** Add up a single category yourself, or compare the AI's total spending with your bank's monthly figure.
- **Ask it to calculate with code.** ChatGPT, Claude and Gemini can run calculations on uploaded files; asking "use code to calculate" makes arithmetic errors less likely.
- **Watch the signs.** Some banks show spending as negative numbers, others as positive with a separate column. Tell the AI which.
- **Look for refunds and transfers.** A refund categorized as income, or a transfer to savings counted as spending, can skew a category.
- **Read the "unsure" list.** Ambiguous merchant names are where wrong categories hide.

## Keep it going each month

A budget only works if you look at it again. A simple routine:

1. At the start of the month, keep your spreadsheet with this month's targets.
2. At the end, download the month's transactions and run the **monthly check-in** prompt.
3. Adjust one or two targets, not everything at once.

Because chatbots don't reliably remember past conversations, paste last month's budget table into the chat each time, or keep everything in a ChatGPT project or a Claude project so the files stay together.

## FAQ

**Is it safe to upload my bank statement to ChatGPT?**
Remove account numbers and personal details first, and turn off model training in your settings if you don't want your chats used. The chatbot only needs dates, descriptions and amounts to build a budget.

**Which AI is best for budgeting?**
For sorting a CSV and drafting a budget, ChatGPT, Claude and Gemini all do the job on their free plans. The bigger differences are upload limits and whether you want ChatGPT's US-only bank connection.

**Can AI give me financial advice?**
It can explain budgeting methods and run scenarios with your numbers, but it isn't a licensed advisor and doesn't know your full situation. For decisions about debt, taxes or investing, talk to a qualified professional.

**Can I use AI with a budgeting app instead?**
Yes. Many budgeting apps export transactions to CSV, so you can run the same prompts on their data. You can also ask an AI to explain or reorganize the categories your app already uses.

**What if my bank only gives PDF statements?**
Upload the PDF and ask the AI to "extract every transaction into a table with date, description and amount." Check that the row count matches the statement before you categorize.

**Can AI build me a budget spreadsheet?**
Yes. Ask for a template with formulas (prompt 5 above). ChatGPT and Claude can also create a downloadable spreadsheet file if you ask for one.

## Sources

- [OpenAI: ChatGPT for personal finance and budgeting](https://openai.com/index/personal-finance-chatgpt/) (May 2026)
- [Analytics Insight: ChatGPT Finances expands to Mac and all personal plans in the US](https://www.analyticsinsight.net/news/chatgpt-finances-hits-mac-us-users-get-4-plan-access) (November 2026)
- [OpenAI Help Center: File uploads FAQ](https://help.openai.com/en/articles/8555545-file-uploads-faq)
- [Claude Help Center: Upload files to Claude](https://support.claude.com/en/articles/8241126-upload-files-to-claude)
- [Gemini Apps Help: Upload and analyze files](https://support.google.com/gemini/answer/14903178)
- [Gemini Apps Help: Limits and feature availability](https://support.google.com/gemini/answer/16275805)
