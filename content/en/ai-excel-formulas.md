---
title: "How to Use AI to Write Excel Formulas (Free and Built-In Options)"
description: "Get working Excel and Google Sheets formulas from ChatGPT, Claude, Gemini or Copilot. How to describe your sheet, copy-paste prompts, fixing errors, and how to check the result."
date: 2026-10-24
key: ai-excel-formulas
tags: [spreadsheets, excel, google-sheets, copilot, gemini, chatgpt, claude]
cover: /images/ai-excel-formulas.svg
coverAlt: "A plain-English request turning into a spreadsheet formula in a highlighted cell"
---

You don't need to memorize XLOOKUP or SUMIFS anymore. Any AI chatbot can write a spreadsheet formula if you tell it three things: what your columns are, where the data sits, and what answer you want in which cell. The quality of the formula depends almost entirely on how clearly you describe the sheet, not on which AI you use.

> **Quick answer:** Open ChatGPT, Claude or Gemini (free plans work). Describe your sheet like this: "Column A has dates in A2:A500, column C has amounts. In F2, I want the total of column C for the month typed in E2." Say whether you use Excel or Google Sheets. Paste the formula into your cell, then test it on a few rows you can check by hand. If you pay for Microsoft 365 with Copilot or a Google plan that includes Gemini, you can also ask inside the spreadsheet itself.

## Your options at a glance

As of October 2026, from each company's help pages:

| Option | Cost | Where you ask | Sees your file? |
|---|---|---|---|
| **ChatGPT, Claude or Gemini chat** | Free plans are enough for formulas | A browser tab next to your spreadsheet | Only what you paste or upload |
| **Copilot in Excel** | Needs Microsoft 365 Personal or Family with an AI credits plan, Microsoft 365 Premium, or an eligible business plan | Copilot pane inside Excel | Yes, the open workbook |
| **Gemini in Google Sheets** | Needs an eligible Google Workspace or Google AI plan | Type `=` in a cell, or the Gemini side panel | Yes, the open sheet |

Two things worth knowing:

- **The `=COPILOT()` cell function is gone.** Microsoft's support page says it stopped working in Excel on September 14, 2026; old workbooks that used it now show `#NAME?` on recalculation. Copilot itself still works through the Copilot pane.
- **Gemini in Sheets can fix broken formulas.** When a cell shows an error, hover over it and click **Fix**, and Gemini reviews the formula and explains the problem. It works best with native Google Sheets files, so save an uploaded .xlsx as a Google Sheet first.

If you have neither paid plan, the free chatbot route below does the same job with one extra step: copy and paste.

## Step by step with a free chatbot

1. **Look at your sheet and write down the layout.** Which column holds what, which row the data starts on (usually row 2 if row 1 has headers), and roughly where it ends.
2. **Say which program and version you use.** "Excel 365", "Excel 2016" or "Google Sheets". Newer functions like `XLOOKUP` and `FILTER` don't exist in older Excel versions, and a few functions differ between Excel and Sheets.
3. **Describe the result, not the formula.** "In D2, show 'Late' if the date in C2 is after today and the status in E2 isn't 'Paid'." You don't need to know the function names.
4. **Ask for an explanation along with the formula.** You'll catch wrong assumptions faster.
5. **Paste it into one cell first.** Check the answer on two or three rows you can work out yourself, then fill the formula down.
6. **If it errors, paste the error back** with the formula and a few sample rows. Let the AI fix it in the same chat.

## Copy-paste prompts

**1. The basic formula request**

> I use [Excel 365 / Excel 2019 / Google Sheets]. My sheet has headers in row 1 and data in rows 2 to [last row]. Columns: A = [what], B = [what], C = [what]. In cell [cell], I want [the result in plain words]. Give me the formula, explain each part in one line, and tell me any assumption you made about my data.

**2. Look up a value from another table**

> In Sheet1, column A has product codes. In a sheet called Prices, column A has the same codes and column B has prices. In Sheet1 column D, I want the matching price for each code, and "Not found" if the code isn't in Prices. I use [program/version].

**3. Sum or count with conditions**

> Column A has dates, column B has the salesperson's name, column C has the amount. In G2, I want the total amount for the name typed in F2, only for dates in the month typed in E2 (as a date like 1/10/2026). Use a formula that works in [program/version].

**4. Fix a formula that isn't working**

> This formula returns [the error, for example #N/A or #VALUE!, or the wrong number]: `[paste formula]`. Here are 5 sample rows from my data, with the column letters: [paste rows]. What's wrong, and what's the corrected formula?

**5. Explain a formula someone else wrote**

> Explain this formula step by step in plain English, as if I've never used these functions: `[paste formula]`. Then tell me what would break it.

**6. Clean messy text**

> Column A has full names like "garcía, MARÍA " with extra spaces and mixed capitals. In column B I want "María García". Give me a formula, and say if it needs a newer Excel version.

## Example: what a good answer looks like

Say you ask: "Column A has order dates, column C has amounts. In F2, total column C for the month of the date in E2. Excel 365."

A correct answer is something like:

```
=SUMIFS(C:C, A:A, ">="&EOMONTH(E2,-1)+1, A:A, "<="&EOMONTH(E2,0))
```

`EOMONTH(E2,-1)+1` is the first day of that month, and `EOMONTH(E2,0)` is the last day, so `SUMIFS` adds every amount whose date falls between them. A good AI answer will explain it roughly that way. If yours doesn't explain, ask.

## Using Copilot or Gemini inside the spreadsheet

The built-in assistants save the copy-paste step because they can see your columns. The prompts are the same; you can just refer to column headers by name.

- **Copilot in Excel:** open the **Copilot** button on the Home tab and ask, for example, "Add a column that shows the number of days between Order Date and Ship Date." Microsoft's help page lists formula generation among its features and tells you to review and verify anything it creates. It needs the workbook in a modern format such as .xlsx, and calculation set to **Automatic**.
- **Gemini in Sheets:** in any cell, type `=` and describe what you want, or open Gemini and ask "Create a formula that divides Goals by Games." You need to be on a computer; it's a desktop feature.

If the spreadsheet belongs to your employer or school, check its policy before pasting work data into a personal chatbot account; many organizations only allow the AI tools they provide.

## How to check an AI formula before you trust it

AI formulas often look right and are quietly wrong. Before relying on one:

- **Test on rows you can calculate yourself**, including an edge case: a blank cell, a zero, a date at the very end of a month.
- **Check the ranges.** A formula that uses `C2:C100` will miss row 101 when your data grows. Ask for whole-column references or an Excel Table if your data changes.
- **Watch for text that looks like numbers or dates.** Imported data often stores "2026-10-01" as text, which makes date formulas return 0. Ask the AI how to convert it.
- **Look for regional differences.** In many European and Latin American locales, Excel uses semicolons instead of commas between arguments (`=SUM(A1;A2)`) and may use localized function names. Tell the AI your region if pasted formulas fail.
- **Don't let it guess your layout.** If the AI says "assuming your data is in column B," and it isn't, correct it and ask again.

## FAQ

**Can ChatGPT write Excel formulas for free?**
Yes. The free plans of ChatGPT, Claude and Gemini all write and explain formulas. You copy the result into Excel or Sheets yourself.

**Do I need Copilot to use AI in Excel?**
No. Copilot puts the assistant inside Excel, but as of October 2026 it requires a qualifying Microsoft 365 plan. Any free chatbot can write the same formulas if you describe your sheet.

**What happened to the =COPILOT function?**
Microsoft retired it on September 14, 2026. Workbooks that used it keep cached results but show `#NAME?` when they recalculate. Use the Copilot pane instead, or replace those cells with regular formulas.

**Can I upload my spreadsheet to ChatGPT instead of describing it?**
Yes. ChatGPT supports .xls, .xlsx and .csv files for data analysis, and Claude and Gemini also accept file uploads. For writing a single formula, though, describing the columns and pasting a few sample rows is often faster and shares less data.

**Why does the formula work in Google Sheets but not in Excel (or the other way around)?**
Most common functions are the same, but some aren't, and older Excel versions lack newer functions like `XLOOKUP`, `FILTER` and `TEXTSPLIT`. Always name your program and version in the prompt.

**Can AI write macros or Apps Script too?**
Yes, chatbots can write VBA macros for Excel and Apps Script for Google Sheets. Only run code you understand or have tested on a copy of the file, because a macro can change or delete data.

**Is it safe to paste my data into an AI chatbot?**
Leave out personal or confidential data you don't need. For formulas, fake sample rows with the same layout work just as well as the real thing.

## Sources

- [Microsoft Support: What is Copilot in Excel?](https://support.microsoft.com/en-us/Excel/copilot/frequently-asked-questions-about-copilot-in-excel)
- [Microsoft Support: COPILOT function](https://support.microsoft.com/en-us/excel/copilot-function)
- [Microsoft Support: AI credits and limits for Microsoft 365 subscriptions](https://support.microsoft.com/Microsoft-365-Copilot/ai-credits-and-limits-for-microsoft-365-subscriptions)
- [Google Docs Editors Help: Gemini in Google Sheets](https://support.google.com/docs/answer/14356410)
- [Google Docs Editors Help: Gemini in Sheets features](https://support.google.com/docs/answer/14218565)
- [OpenAI Help Center: Data analysis with ChatGPT](https://help.openai.com/en/articles/8437071-data-analysis-with-chatgpt)
