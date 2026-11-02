---
title: "How to Translate a Document with AI (and Keep the Formatting)"
description: "Translate a Word, PDF or PowerPoint file with AI: when to use Google Translate, DeepL, Word or Google Docs, and when ChatGPT, Claude or Gemini do it better. Free limits and prompts."
date: 2026-11-02
key: translate-document-with-ai
tags: [translation, documents, chatgpt, claude, gemini, beginner]
cover: /images/translate-document-with-ai.svg
coverAlt: "A document in one language turning into the same document in another language, with the layout unchanged"
---

There are two kinds of AI tools that can translate a document, and they're good at different things. **Document translators** (Google Translate, DeepL, and the translate buttons in Word and Google Docs) take your file and give back the same file in another language, with the layout intact. **AI chatbots** (ChatGPT, Claude, Gemini) give you more control over tone, terminology and audience, but they work best on the text rather than the layout.

> **Quick answer:** If you need the same file back with the formatting kept, upload it to **Google Translate** (translate.google.com, then **Documents**) or **DeepL**, or use **Tools > Translate document** in Google Docs or **Review > Translate > Translate Document** in Word. If the wording matters more than the layout (a letter, a website text, a school assignment, a message to a client), paste or upload the text into ChatGPT, Claude or Gemini and tell it who the reader is and what tone to use. For anything legal, medical or official, have a qualified human check the result.

## Which tool to use

| What you need | Best fit | Why |
|---|---|---|
| Same Word, PowerPoint, Excel or PDF file, layout kept | Google Translate or DeepL | Upload the file, download a translated copy in the same format |
| You already work in Word (Microsoft 365) | Word: **Review > Translate > Translate Document** | Creates a translated copy and leaves the original unchanged |
| You already work in Google Docs | Google Docs: **Tools > Translate document** | Free, saves the translated copy in your Google Drive |
| Natural tone, specific audience, consistent terms | ChatGPT, Claude or Gemini | You can explain context, give a glossary and ask for revisions |
| Short text you just need to understand | Any of the above | For "what does this say?", even a quick paste is enough |

Many people combine the two: translate the file with a document translator to keep the layout, then paste the important paragraphs into a chatbot to polish the wording.

## Free limits for document translators (as of November 2026)

These come from each company's own help or pricing pages. Limits change, so check the linked pages if an upload fails.

| | Google Translate | DeepL Free | Word (Microsoft 365) | Google Docs |
|---|---|---|---|---|
| **File types** | .docx, .pdf, .pptx, .xlsx | Word, PowerPoint, Excel, PDF and more | Word documents | Google Docs files |
| **Size limit** | 10 MB per file; PDFs up to 300 pages | Up to 5 MB per file | Not published | Not published |
| **How many** | No monthly cap published | 1 file translation per month | Not published | Not published |
| **Cost** | Free | Free plan; paid plans allow more files and up to 30 MB per file | Included with a Microsoft 365 subscription | Free with a Google account |

DeepL's free plan is fine for a one-off file but quickly runs out if you translate documents every week. Google Translate and the Google Docs feature have no published monthly cap.

## How to translate a file with Google Translate

1. Go to **translate.google.com** in your browser.
2. At the top, click **Documents**.
3. Choose the language to translate from (or leave it on detect) and the language to translate to.
4. Click **Browse your computer** and select your file (.docx, .pdf, .pptx or .xlsx, up to 10 MB).
5. Click **Translate**, wait for it to finish, then click **Download translation**.

If your PDF is over 300 pages or 10 MB, split it into parts first and translate each part.

## How to translate inside Word or Google Docs

**Word (Microsoft 365, Mac or web):** open the document, go to the **Review** tab, click **Translate**, then **Translate Document**, and choose the target language. Word creates a new copy in that language, so your original stays as it was.

**Google Docs:** open the document, click **Tools > Translate document**, give the copy a name, choose the language and click **Translate**. The translated copy opens in a new window and is saved in your Drive. If you don't see the option, the file is probably a Word file being edited in Docs; use **File > Save as Google Docs** first.

## How to translate a document with ChatGPT, Claude or Gemini

Chatbots shine when the translation has to *sound right* for a specific reader, not just be accurate word for word.

1. **Upload the file or paste the text.** Use the **+** or paperclip button next to the message box. As of November 2026, ChatGPT's free plan allows 3 file uploads per day; Gemini accepts files up to 100 MB; Claude accepts PDFs and other documents on its free plan.
2. **Give context.** Who will read it, what the document is for, and which variety of the language you need (for example, Spanish for Mexico or Spanish for Spain, Brazilian or European Portuguese, UK or US English).
3. **Ask for the format you want back.** A clean translation, a side-by-side table, or a file. Claude can create Word (.docx) and PDF files on all plans, including Free, so you can ask it to "give me the translation as a Word document". In any tool, you can also copy the result into your own document.
4. **Translate long documents in parts.** For anything longer than a few pages, ask for one section at a time so nothing gets skipped or summarized.
5. **Review.** Ask the AI to list sentences it was unsure about, then check those yourself or with a native speaker.

## Copy-paste prompts

**General translation with the right tone**

> Translate the attached document from [source language] into [target language] for [reader, e.g. "parents at a school in Mexico" or "a client in Germany"]. Keep the meaning exact, but make it sound natural, as if it were written in [target language] originally. Keep headings, lists and numbers as they are. Don't summarize or skip anything.

**Consistent terminology (glossary)**

> Translate this into [language]. Use these fixed translations every time: [term] = [translation], [term] = [translation]. Leave product names, brand names and anything in ALL CAPS untranslated. At the end, list any other terms where you had to choose between two translations.

**Side-by-side check**

> Translate this document into [language] as a two-column table: original sentence on the left, translation on the right. Mark with ⚠️ any sentence where the meaning is ambiguous or where you made an assumption.

**Long document, one part at a time**

> This document has several sections. First, list the section headings. Then translate only section 1 in full. Wait for me to say "next" before translating the next section.

**Back-translation to catch errors**

> Here is a translation into [language]. Translate it back into [original language] as literally as possible, so I can compare it with the original and spot meaning changes.

## Formatting tips

- **Scanned PDFs** are pictures of text. Document translators may return little or nothing. Run OCR first (for example, open the PDF from Google Drive with Google Docs), or upload clear page images to a chatbot.
- **PDFs often come back with shifted layout**, because translated text is longer or shorter than the original. If the layout matters, translate the original Word or PowerPoint file instead of the PDF when you can.
- **Spreadsheets:** if you only need to translate one column (product names, survey answers), paste that column into a chatbot and ask for a column back in the same order, or use the `GOOGLETRANSLATE` function in Google Sheets.
- **Text inside images, charts and logos** usually isn't translated by any of these tools. Recreate those by hand.

## Privacy: check before you upload

Uploading a document sends it to the company that runs the tool. Avoid uploading contracts, medical records, ID documents or confidential work files unless your employer or school has approved that tool. Check each tool's privacy or data settings, and remove personal details you don't need translated.

## When AI translation isn't enough

AI translation is good enough to understand a document, write everyday messages and get a solid first draft. It is not a substitute for a **certified translation** when one is required, for example for immigration, court, university admission or official records. Those usually need a sworn or certified translator, so check what the receiving office accepts before you send anything. For medical instructions, legal terms and safety information, have a qualified person review the translation.

## FAQ

**What is the best free way to translate a whole document?**
For a Word, PowerPoint, Excel or PDF file, Google Translate's **Documents** tab is the simplest free option: up to 10 MB per file and 300 pages per PDF, as of November 2026. If your file is in Google Docs, use **Tools > Translate document**.

**Is ChatGPT better than Google Translate for documents?**
They do different jobs. Google Translate returns the same file with the layout kept. ChatGPT (like Claude and Gemini) lets you set the tone, audience and terminology, which often gives more natural wording, but you'll usually rebuild the layout yourself or ask for a new file.

**Can AI translate a PDF and keep the layout?**
Google Translate and DeepL return a translated PDF, but complex layouts can shift because translated text changes length. You'll get better results translating the original Word or PowerPoint file if you have it.

**Is AI translation accurate?**
For common language pairs and everyday text, it's usually accurate enough to rely on for understanding and drafts. It can still mistranslate idioms, names, numbers, legal terms and ambiguous sentences, so check anything important.

**Can I use an AI translation for official documents?**
Usually not on its own. Many official processes require a certified or sworn translation. Use AI to understand the document, then get a certified translation if the receiving office requires it.

**Why won't my file upload to Google Translate?**
The usual reasons are that it's over 10 MB, a PDF over 300 pages, password-protected, or not one of the supported formats (.docx, .pdf, .pptx, .xlsx). Compress or split it, remove the password, or save it in a supported format.

## Sources

- [Google Translate Help: Translate documents & websites](https://support.google.com/translate/answer/2534559?co=GENIE.Platform%3DDesktop&hl=en)
- [Google Docs Editors Help: Translate documents or write in a different language](https://support.google.com/docs/answer/187189?hl=en)
- [Microsoft Support: Translate text into a different language](https://support.microsoft.com/en-us/article/abb961ba-4f3e-4fe9-a0bc-7feddbe64860)
- [DeepL: plans and pricing](https://www.deepl.com/en/pro)
- [DeepL Pro Service Specification](https://www.deepl.com/pro-service-specifications)
- [OpenAI Help Center: File Uploads FAQ](https://help.openai.com/en/articles/8555545-file-uploads-faq)
- [Claude Help Center: Create and edit files with Claude](https://support.claude.com/en/articles/12111783-create-and-edit-files-with-claude)
- [Gemini Apps Help: Upload & analyze files in Gemini Apps](https://support.google.com/gemini/answer/14903178)
