---
title: "How to Analyze Spreadsheet Data with AI (Free Options)"
description: "Upload a CSV or Excel file to ChatGPT, Claude or Gemini and get totals, trends and charts in plain English. Steps, file limits, copy-paste prompts and how to check the numbers."
date: 2026-11-23
key: analyze-spreadsheet-data-with-ai
tags: [spreadsheets, data-analysis, excel, csv, chatgpt, claude, gemini]
cover: /images/analyze-spreadsheet-data-with-ai.svg
coverAlt: "A spreadsheet file turning into a bar chart and a short written summary"
---

You can hand a spreadsheet to an AI chatbot and ask questions about it in plain English: "Which product sold best last quarter?", "Is anything unusual in these expenses?", "Make a chart of monthly sales." ChatGPT, Claude and Gemini can all read uploaded CSV and Excel files, and ChatGPT and Claude actually run code on your data to calculate the answer instead of guessing at it. The catch is that the AI only knows what is in the file, and it can still misread a column, so you need to check its work.

> **Quick answer:** Clean up your file so row 1 has clear column names, save it as .csv or .xlsx, and upload it to ChatGPT, Claude or Gemini (all have free plans that accept files, with lower limits). Start with "Describe this data: what each column contains, the date range and any problems you notice." Then ask your real questions one at a time, ask for a chart if you want one, and spot-check two or three numbers against the sheet yourself before you use the results.

## Which AI to use

All three main chatbots accept spreadsheets. As of November 2026, according to each company's help pages:

| | ChatGPT | Claude | Gemini |
|---|---|---|---|
| **Spreadsheet types** | .xls, .xlsx, .csv | CSV, TSV, Excel and other files | Most file types, including spreadsheets |
| **Size limit** | About 50 MB for CSV and spreadsheet files (depends on row size) | 30 MB per file | 100 MB per file |
| **Runs code on your data?** | Yes (Python) | Yes, when code execution is turned on | Analyzes the file; charts on the web app |
| **Charts** | Static image charts; bar, line, pie and scatter can be interactive | Charts as image files, or inside an Excel file it creates | Ask for a chart from an attached spreadsheet in the web app |
| **Free plan** | Yes, with a smaller upload allowance | Yes, code execution is available on all plans | Yes, with lower limits; Google AI plans raise them |

Which one to pick matters less than how you ask. A few practical differences:

- **ChatGPT** shows the tables it builds as interactive tables you can scroll and sort, and lets you switch some charts between static and interactive.
- **Claude** can hand back a new Excel file (for example, your data with a summary sheet and a chart added). On the Free, Pro and Max plans you may need to switch on **Code execution and file creation** (shown as **Create and edit files** in newer layouts) under **Settings > Capabilities**.
- **Gemini** works well if your files already live in Google Drive, because you can attach them from Drive. Work and school accounts may need an administrator to allow it.

If you pay for Microsoft 365 with Copilot or a Google plan with Gemini in Sheets, you can also ask questions inside Excel or Google Sheets without uploading anything. Our guide to [writing Excel formulas with AI](/ai-tools-guide/en/ai-excel-formulas/) covers those built-in options and their plan requirements.

## Step by step

1. **Make a copy of the file.** Work on the copy, and remove columns you don't need, especially names, emails, phone numbers or account numbers.
2. **Fix the layout.** One header row, one row per record, no merged cells, no blank rows in the middle, no subtotal rows mixed into the data. Charts and notes on the sheet are best removed. AI tools read a clean table far more reliably than a formatted report.
3. **Use clear column names.** "Order date", "Region", "Revenue (EUR)" beats "Col F" or "Rev2". Include the unit or currency in the name.
4. **Save as .csv or .xlsx.** CSV is the safest choice if your workbook has many tabs or complex formulas; ChatGPT's help page notes that the number and complexity of formulas can slow processing even when the file is under the size limit. Export one tab per CSV.
5. **Upload and ask for a description first.** Before any real question, ask the AI to list the columns, the number of rows, the date range and any missing or odd values. If its description is wrong, its answers will be too.
6. **Ask one question at a time.** "Total revenue by month for 2026" is better than a list of ten questions. Follow up in the same chat so it keeps the context.
7. **Ask for a chart only when you know what you want it to show.** "Line chart of monthly revenue, one line per region" gets a better result than "make a chart".
8. **Check the numbers** (see the checklist below) before you paste anything into a report.
9. **Ask for the results as a file** if you need them in your spreadsheet: a CSV of the summary table, or, in Claude, an .xlsx with the summary on a new sheet.

## Copy-paste prompts

Start every analysis with this:

```
I've uploaded a spreadsheet. Before answering anything, describe it:
- What each column contains and its data type
- How many rows there are and the date range, if there are dates
- Any missing values, duplicates, typos in categories or numbers stored as text
Don't change anything yet. Ask me if a column's meaning is unclear.
```

Basic summary:

```
Using this data, give me:
1. Total [revenue] by [month]
2. The top 5 [products] by [revenue], with their share of the total
3. Anything that changed sharply from one [month] to the next
Show your results as a table and tell me exactly how you calculated each one.
```

Cleaning messy data:

```
Clean this data and give me a new CSV file:
- Standardize the [Country] column (e.g. "USA", "U.S." and "United States" become one value)
- Convert the [Date] column to YYYY-MM-DD
- Remove exact duplicate rows
List every change you made and how many rows were affected.
```

Comparing two periods or groups:

```
Compare [Q3 2026] with [Q3 2025]: total [sales], number of [orders] and average [order value].
Break it down by [region]. Point out the biggest changes and possible reasons
that are visible in the data itself. Don't guess at causes the data can't show.
```

Charts:

```
Make a [bar chart] of [total expenses] by [category] for [2026], sorted from largest to smallest.
Label each bar with its value. Use the column names as axis labels.
```

Finding problems:

```
Check this data for anything that looks wrong: negative amounts, dates in the future,
values far outside the normal range, or rows that don't add up.
List each suspicious row with the reason, but don't delete anything.
```

Replace the words in brackets with your own column names. Using the exact header text from your file helps the AI pick the right column.

## Example: a small business sales file

Say you run an online shop and export your orders as a CSV with the columns *Order date*, *Product*, *Category*, *Quantity*, *Unit price* and *Country*. A useful first session might look like this:

1. Ask for the description prompt above. The AI reports, for example, that *Unit price* has a few rows stored as text and that *Country* has both "UK" and "United Kingdom".
2. Ask it to clean those two issues and confirm how many rows changed.
3. Ask: "Revenue (Quantity × Unit price) by month and by category, as a table."
4. Ask: "Line chart of monthly revenue, one line per category."
5. Ask: "Which three products had the biggest drop in revenue from the first half of the year to the second half?"
6. Check one month's total yourself with a SUM in your spreadsheet.

Notice that step 3 tells the AI how revenue is calculated. If your file has no revenue column, never assume it will compute it the way you would.

## How to check AI analysis before you trust it

AI tools that run code are usually right about arithmetic, but they can be wrong about what your data means. Before you use a result:

- **Recompute one or two numbers yourself.** A quick SUM, COUNT or pivot table in Excel or Sheets on the same rows.
- **Check the row count.** If your sheet has 4,312 rows and the AI says it analyzed 4,000, ask why.
- **Watch for misread columns.** Dates read as text, US vs European date formats (03/04 can be March 4 or April 3), commas vs dots as decimal separators, and currency symbols inside numbers are the most common traps.
- **Ask how it calculated.** "Show the code you used" (ChatGPT, Claude) or "explain step by step how you got this number". If it filtered out rows, it should say which ones.
- **Be skeptical of explanations.** The data can show *that* sales dropped in August; it usually cannot show *why*. Treat any reason the AI offers as a guess unless it points to a column that supports it.
- **Re-run important questions in a new chat.** If you get a different answer, something is ambiguous in your data or your question.

## What AI is not good at here

- **Very large files.** Files above the size limits won't upload, and big files near the limit can be slow or fail. Filter or split the data first, or summarize it in a pivot table and upload that.
- **Scanned tables and screenshots.** ChatGPT's help page warns it may not reliably extract exact values from image-based tables or scanned files. Use the original spreadsheet when you can.
- **Live data.** The AI analyzes the file you uploaded, not your current numbers. ChatGPT's analysis environment, for example, cannot make web requests. Upload a fresh export when the data changes.
- **Decisions.** It can summarize; you still decide what the numbers mean for your business, budget or project.

## FAQ

**Can I analyze an Excel file with ChatGPT for free?**
Yes. ChatGPT's free plan accepts file uploads, including .xls, .xlsx and .csv, but with a smaller upload allowance than paid plans. Claude and Gemini also accept spreadsheets on their free plans.

**Which is best for data analysis: ChatGPT, Claude or Gemini?**
For everyday questions about a single spreadsheet, all three do the job. ChatGPT and Claude run code on the file, which makes calculations more dependable and lets them return cleaned files. Gemini is convenient if your files are in Google Drive and accepts larger files (100 MB vs 30 MB for Claude, as of November 2026).

**Is it safe to upload my spreadsheet to an AI?**
Remove anything personal or confidential you don't need for the question, and check your account's data settings. Our guide on [stopping AI from training on your chats](/ai-tools-guide/en/stop-ai-training-on-your-chats/) shows where those settings are. For work data, follow your employer's rules on which AI tools are approved.

**Why does the AI give a different total than my spreadsheet?**
Usually because it read a column differently: numbers stored as text were skipped, dates were parsed in the wrong format, or a subtotal row was counted twice. Ask it to list the rows it included and compare.

**Can AI make a pivot table for me?**
It can build the same summary table a pivot table would and give it to you as a CSV or Excel file. To get a real, refreshable pivot table in your workbook, ask the AI for step-by-step instructions for Excel or Google Sheets, or use Copilot or Gemini inside the spreadsheet if your plan includes them.

**My file is too big to upload. What can I do?**
Delete columns you don't need, filter to the period you care about, split it into smaller CSVs, or create a summary in your spreadsheet first and upload that.

## Sources

Facts checked against these pages in November 2026:

- [OpenAI Help Center: Data analysis with ChatGPT](https://help.openai.com/en/articles/8437071-data-analysis-chatgpt)
- [OpenAI Help Center: File uploads FAQ](https://help.openai.com/en/articles/8555545-file-uploads-faq)
- [Claude Help Center: Create and edit files with Claude](https://support.claude.com/en/articles/12111783-create-and-edit-files-with-claude)
- [Gemini Apps Help: Upload and analyze files in Gemini Apps](https://support.google.com/gemini/answer/14903178)
