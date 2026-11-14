---
title: "How to Take Meeting Notes with AI (Zoom, Google Meet, Teams)"
description: "Get automatic AI meeting notes and action items in Zoom, Google Meet or Microsoft Teams, which plans include it, and a free method for any meeting. Steps and prompts."
date: 2026-11-14
key: ai-meeting-notes
tags: [meetings, notes, work, zoom, google-meet, teams, gemini, copilot, chatgpt, claude]
cover: /images/ai-meeting-notes.svg
coverAlt: "A video call window turning into a short list of notes and checked action items"
---

Taking notes while you're also trying to listen and talk is hard, and it's exactly the kind of job AI does well: it can listen to the whole meeting, then hand you a summary, the decisions and a list of who agreed to do what. The catch is that the built-in options depend on which meeting app you use and which plan you're on, and the notes still need a human check before anyone acts on them.

> **Quick answer:** In **Zoom**, the host clicks the **Zoom AI** icon, ticks **Meeting summary** and clicks **Start Zoom AI**; the summary arrives by email after the call (free Basic accounts get this for 3 hosted meetings a month, paid Pro gets unlimited). In **Google Meet**, click **Take notes for me** in the top right; notes are saved to the organizer's Google Drive (needs an eligible work or school account, or Google AI Pro or Ultra). In **Microsoft Teams**, open the meeting's **Recap** tab afterwards (needs Teams Premium or a Microsoft 365 Copilot license, and transcription turned on). With none of these, transcribe the meeting and paste the transcript into a free chatbot with the prompt below.

Plans, prices and steps below are as of November 2026 and come from Zoom's, Google's and Microsoft's own help and pricing pages (linked at the end).

## Which option fits you

| You use | Built-in AI notes | What you need (as of November 2026) | Where the notes end up |
|---|---|---|---|
| Zoom | Meeting summary | Free Basic: 3 hosted meetings per month. Pro ($16.99/user per month billed monthly, US) and higher: unlimited | Email to the host (and to participants if the host shares it), plus the meeting's group chat |
| Google Meet | Take notes for me (Gemini) | An eligible Google Workspace work or school edition, or a personal Google AI Pro ($19.99/month, US) or Ultra plan | A Google Doc in the organizer's Drive, attached to the Calendar event |
| Microsoft Teams | Intelligent recap (Copilot) | A Teams Premium or Microsoft 365 Copilot license, with transcription allowed by your admin | The Recap tab of the meeting in Teams chat and calendar |
| Anything else (phone call, in-person, other apps) | None needed | A transcript or recording plus any chatbot (ChatGPT, Claude, Gemini, Copilot) | Wherever you paste it |

If you're on a work or school account, the meeting organizer's license usually decides whether the feature is available, and your IT admin can switch it off. If you don't see the button, ask them before installing an extra tool.

## How to get AI notes in Zoom

Zoom's AI assistant is called AI Companion in Zoom's help pages and ZoomMate on its newer product pages. The meeting summary feature works the same way.

1. Start the meeting as the **host** (only the host or a co-host can start or stop it; participants can ask the host to turn it on).
2. On desktop, hover over the **Zoom AI** icon in the top-right corner. On mobile, tap the Zoom AI icon.
3. Tick **Meeting summary**. Optionally tick **Generate transcript** if you also want the full text.
4. Click **Start Zoom AI**.
5. After the meeting, the summary is emailed to you and, if chat is enabled, posted in the meeting's group chat. Only the host can edit or delete it.

Good to know:

- Zoom writes the summary in the language most participants spoke (or the host's language if there's no majority).
- Participants who were signed in can receive the summary automatically if the host chooses to share it. People who joined without signing in don't get the email.
- It doesn't work in breakout rooms, and no recording is required.
- Users with Basic permissions on a paid company account don't get the AI features; that's set by the account owner.

## How to get AI notes in Google Meet

Google calls the feature **Take notes for me**, powered by Gemini.

1. Join the meeting at meet.google.com.
2. Click **Take notes for me** in the top-right corner.
3. Optional: open **Settings** to choose who receives the notes (**Send notes to**), the **Notes length** (Standard or Longer) and which sections to include.
4. Click **Start taking notes**. Everyone in the call sees a pencil icon and a notice that notes are being taken.

You can also switch it on ahead of time: in Google Calendar, edit the event, open **Video call options > Meeting records** and tick **Take notes with Gemini**.

After the call, a Google Doc with two tabs, **Quick notes** and **Full notes**, is saved in the organizer's Drive in a "Google Meet" folder, attached to the Calendar event, and emailed to the chosen recipients.

Good to know (as of November 2026):

- Supported meeting languages are English, French, German, Italian, Japanese, Korean, Portuguese and Spanish, one language per meeting.
- Google recommends it for meetings between 15 minutes and 8 hours long.
- Since August 2026 there's also a version for **in-person meetings**: tap **Take notes** on the Meet home screen (web or mobile), put your device on the table, and stop it when you're done. You get a summary, action items and a transcript in a Google Doc. Google lists it for Business Standard and Plus, Enterprise Standard and Plus, Frontline Plus, Google AI Pro for Education, and personal Google AI Pro and Ultra.
- Google's pages list Google AI Pro and Ultra as the personal plans that include it. If you're on the cheaper Google AI Plus, check whether the button appears before you rely on it.

## How to get AI notes in Microsoft Teams

Teams calls it **intelligent recap**.

1. Make sure you have the license: a Microsoft 365 plan that includes Teams, plus **Teams Premium** or a **Microsoft 365 Copilot** license. Your admin must also allow transcription.
2. Hold the meeting as usual. For the richest recap, record and transcribe it.
3. When the meeting ends, open it from the Teams chat or calendar and select the **Recap** tab.

The recap can include AI notes, suggested tasks with owners, and markers on the timeline showing when your name was mentioned or when a topic started. If the meeting wasn't recorded, you still get the AI notes but not the recording, chapters or speaker timeline. With a Microsoft 365 Copilot license, scheduled meetings can get a recap without saving a transcript, and you can also listen to an audio recap (in preview as of November 2026).

In large Teams events, only organizers, co-organizers and presenters get the recap, not attendees.

## The free method: any meeting, any app

No paid plan? You can still get good notes in two steps.

**Step 1: Get a transcript.** Use your meeting app's own transcript if it has one, or record (with everyone's permission) and transcribe the file. Our guide on [how to transcribe audio to text with AI](https://hwancole.github.io/ai-tools-guide/en/transcribe-audio-with-ai/) covers free ways to do this, including Microsoft Word on the web and Gemini.

**Step 2: Paste it into a chatbot.** ChatGPT, Claude, Gemini and Copilot all have free tiers that can handle a typical meeting transcript. Very long meetings may hit free-plan limits; if that happens, split the transcript in half and summarize each part.

## Copy-paste prompts

**1. Standard meeting notes**

> Here is the transcript of a meeting: [paste]. Write meeting notes with these sections: Summary (3-5 sentences), Decisions made, Action items (task, owner, deadline if mentioned), Open questions. Only use what's in the transcript. If an owner or deadline isn't stated, write "not stated" instead of guessing.

**2. Notes for people who missed it**

> Turn these meeting notes into a short update for teammates who weren't there: [paste]. Under 150 words. Start with what changed or was decided, then what they need to do. Plain language, no jargon.

**3. Follow-up email**

> Draft a follow-up email to the attendees of this meeting based on these notes: [paste]. Thank them briefly, list the decisions and action items with owners, and confirm the next meeting date if one was set. Keep it under 200 words.

**4. Check the AI notes against the transcript**

> Here are AI-generated meeting notes: [paste notes]. And here is the transcript: [paste transcript]. List anything in the notes that isn't supported by the transcript, any action item assigned to the wrong person, and any important point the notes missed.

**5. Prepare for the next meeting**

> Based on these notes from our last meeting: [paste], write an agenda for the follow-up meeting. Include a check-in on each open action item and each unresolved question.

## Before you share AI notes: a quick checklist

- **Names.** AI can mix up who said what, especially when people talk over each other or join from one room.
- **Action items.** Confirm each owner actually agreed to the task. A suggestion isn't a commitment.
- **Numbers and dates.** Check prices, budgets and deadlines against what was said.
- **Tone.** Remove side comments or jokes that made it into the notes and shouldn't be shared.
- **Recipients.** In Zoom and Meet, automatic sharing can send notes to everyone invited. Check the settings before sensitive meetings.

## Privacy and consent

Always tell people when AI is taking notes or a meeting is being recorded or transcribed. On-screen notices are easy to miss, so say it out loud at the start, and in many places recording a conversation without consent is against the law. For confidential meetings (HR, legal, health, customer data), use only the tools your organization has approved, and avoid pasting transcripts into a personal chatbot account. Our guide on [how to stop ChatGPT, Claude and Gemini training on your chats](https://hwancole.github.io/ai-tools-guide/en/stop-ai-training-on-your-chats/) explains the privacy settings for the free method.

## FAQ

**Can I get free AI meeting notes in Zoom?**
Yes, with limits. As of November 2026, Zoom's pricing page lists meeting summaries for 3 hosted meetings per month on the free Basic plan. Paid Pro and higher plans include unlimited meeting summaries.

**Is "Take notes for me" in Google Meet free?**
Not on a regular free Gmail account. It needs an eligible Google Workspace work or school edition, or a personal Google AI Pro or Ultra plan.

**Why can't I see intelligent recap in Teams?**
You need Teams Premium or a Microsoft 365 Copilot license, and your admin must have transcription turned on. If the meeting was a large event and you were an attendee, recap isn't available to you.

**Do other people know AI is taking notes?**
In Google Meet, Google says everyone sees a pencil icon and a notice that notes are being taken. Don't rely on on-screen indicators alone in any app: say it at the start of the meeting, and ask before recording.

**Can AI take notes for an in-person meeting?**
Yes. Google Meet's in-person "Take notes" works from the Meet home screen on eligible plans. Otherwise, record on your phone with everyone's permission, transcribe it, and use the prompts above.

**Are AI meeting notes accurate?**
Usually good for the overall summary, less reliable for exact names, numbers and who agreed to what. Treat them as a first draft and check the action items before sending.

**Which is best: Zoom, Meet, Teams or a chatbot?**
Use whatever your meetings already run on; the built-in option saves the most time. A chatbot is the best fallback when you have no paid plan, or when you want notes in a specific format.

## Sources

- [Zoom Support: Using Meeting Summary with AI](https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0058013)
- [Zoom Workplace pricing](https://zoom.us/pricing)
- [Zoom AI pricing (ZoomMate)](https://zoom.us/pricing/aic)
- [Google Meet Help: Take notes for me in Google Meet](https://support.google.com/meet/answer/14754931?hl=en)
- [Google Workspace Updates: Take notes for me for in-person meetings (August 2026)](https://workspaceupdates.googleblog.com/2026/08/take-notes-with-me-for-in-person-meetings-is-now-available.html)
- [Google AI subscriptions and prices](https://gemini.google/subscriptions/)
- [Microsoft Learn: Intelligent recap for Teams meetings and calls](https://learn.microsoft.com/microsoftteams/intelligent-recap-calls-meetings)
